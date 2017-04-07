# adtask-18-waterfall
原理：利用绝对定位，位置可能不是按照1,2,3顺序排列</b>
1、计算容器内一行可以放置多少元素，方法：容器宽度/元素宽度，取整</b>
2、把每行中的所有元素的高度值存入一个空数组</b>
3、在数组中找出最小高度值的值minValue及其下标minIndex</b>
4、把第二行第一个元素定位到minValue的下面</b>
  top: minValue(包含了包括内边距、边框、外边距的高度值)</b>
  left: minIndex*元素宽度（包含了包括内边距、边框、外边距）</b> 
5、重置当前高度值数组的最小值</b>
6、以此类推</b>

$node.width();//不包括内边距   </b> 
$node.height();//不包括内边距   </b>
$node.innerWidth();//包括内边距   </b>
$node.innerHeight();//包括内边距   </b>
$node.outerWidth();//包括内边距、边框   </b>
$node.outerHeight();//包括内边距、边框   </b>
$node.outerWidth(true);//包括内边距、边框、外边距  </b>
$node.outerHeight(true);//包括内边距、边框、外边距  </b>