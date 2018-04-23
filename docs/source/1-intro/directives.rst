Directives
==========================================

Directives是Roles之外的另一个rst使用的隐式标记，用以拓展它的功能。Directive block包含三个部分：参数（arguments），选项（options，一个rst语法表示的列表)，内容（content）。

它的结构通常是这样的：::

    +-------+-------------------------------+
    | ".. " | directive type "::" directive |
    +-------+ block                         |
            |                               |
            +-------------------------------+

比如插入一个图片：::

    .. image:: http://www.w3school.com.cn//i/eg_tulip.jpg

.. image:: http://www.w3school.com.cn//i/eg_tulip.jpg

插入一个危险提示：::

    .. DANGER::
        Beware killer rabbits!

.. DANGER::
    Beware killer rabbits!

插入一个csv表格：::

    .. csv-table:: Frozen Delights!
       :header: "Treat", "Quantity", "Description"
       :widths: 15, 10, 30

       "Albatross", 2.99, "On a stick!"
       "Crunchy Frog", 1.49, "If we took the bones out, it wouldn't be

.. csv-table:: Frozen Delights!
    :header: "Treat", "Quantity", "Description"
    :widths: 15, 10, 30

    "Albatross", 2.99, "On a stick!"
    "Crunchy Frog", 1.49, "If we took the bones out, it wouldn't be



