角色（Roles）
==========================================

被解释文本（Interpreted text）用
反引号(`)来标记。可以在它前面添加显式标记来改变效果。这就叫做角色（Role）。

比如以下例子：::

    :emphasis:`text`

效果：:emphasis:`text`

我们还可以用directive自定义Role：::

    .. role:: raw-html(raw)
       :format: html

    使用：
    :raw-html:`a<br />b`

.. role:: raw-html(raw)
   :format: html

效果： :raw-html:`a<br />b`
