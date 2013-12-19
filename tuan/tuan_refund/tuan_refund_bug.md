

**后台**


**所有订单** , **已支付订单**

<span style="color:red">1、订单锁定后，跳往锁定订单列表？ 所有订单菜单及已支付订单锁定后，还是留在原页面。</span>

<span style="color:red">2、交易已完成订单这个菜单替换成已支付订单。</span>

<span style="color:red">3、解锁成功后，跳往锁定订单列表？ 所有订单菜单及已支付订单解锁后，留在原页面。</span>

<span style="color:red">4、所有订单列表中，加入一列：订单锁定状态</span>

<span style="color:red">5、已支付订单列表中，加入一列：订单锁定状态</span>

<span style="color:red">6、审请售后页面中，支付是一卡通支付的，退回账号处于可编辑状态【应该是不能编辑的，一卡通和支付宝支付的，都是原路返回】</span>

<span style="color:red">7、申请售后时，没有锁定的订单也能进入售后页面。</span>

<span style="color:red">8、受理页面，弹出框中，商品类型显示错误。</span>

<image src="bug/1-8.png"/>

<span style="color:red">9、点击改为已发货按钮，弹出的div层，显示不了。</span>

<image src="bug/1-9.png"/>


<span style="color:red">10、已发货状态为空！。</span>

<image src="bug/1-10.png"/>
<image src="bug/1-10-1.png"/>

**团购退换货申请**

<span style="color:red">1、售后查看详细页面显示退货单与退款单列表。</span>

<span style="color:red">2、点击关闭售后，状态没有改变。</span>

<image src="bug/4-1.png"/>
<image src="bug/4-1-1.png"/>

**团购待财审退换货**

<span style="color:red">1、售后查看详细页面显示退货单与退款单列表。</span>

<span style="color:red">2、财审时，应显示退款单和退货单列表。</span>



**退货单**

<span style="color:red">1、若退货单完成后，需判断该退货单是否有对应的退款单，若没有，则需更新订单中的back\_status，refund\_num字段</span>

<span style="color:red">2、商品名称空，发货状态空</span>

<image src="bug/2-1.png"/>


<span style="color:red">3、退货单，点击收货并质检，给出提示信息错误。</span>

<image src="bug/2-2-1.png"/>
<image src="bug/2-2-2.png"/>

<span style="color:red">4、退货单列表增加一列：供应商确认状态。</span>


**供应商平台**

<span style="color:red">1、供应商确认失败，给出的提示信息有误。</span>

<image src="bug/3-1.png"/>


<span style="color:red">2、布局由问题，checkbox单独一列。</span>

<image src="bug/3-2.png"/>

<span style="color:red">3、供应商确认收货以后，增加一个判断：若没有对应的退款单，则需将售后单置为已完成状态。</span>
