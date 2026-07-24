#Table Headers
-Table headers are defined using th tag

**To use column as table header**
we need to add th tag in each row(i.e inside tr tag)

**Alignment of table header 
-By default table header is aligned at the center.
-To change alignment of table we use text-align property inside the style tag
    Eg: <style>
        th {text-align:right;}
        </style>

**Merging columns
-Headers can be written over two or more column.
-We use colspan attribute on the th tag
    Eg: <table>
         <tr>
          <th colspan="3">Name</th>
          <th>Age</th>
         </tr>
        </table>

**Captions in table
--Captions can be added in table using the caption tag just after the table tag
    Eg: <table>
    <caption>Student Info</caption>
    </table>

#Padding
**Cell Padding -Space between content and cell edge
   By default it is 0.
   Eg: th,td {
    padding:20px;
   }
   To add padding only above content we use padding-top property.Similarly,padding-bottom,padding-left,padding-right are also used
   Eg: th,td {
    padding-top:20px;
   }
**Cell Spacing-Space between two cells by default it is 2px
It can be set using border-sacing property on table element
Eg: table {
    border-spacing:30px;
}

#Zebra Stripes in Tables
**Zebra Striping -Rows
 Eg: tr:nth-child(even){
    background-color:violet;
  }
  odd can also be written in place of even

**Zebra Striping-Columns
 Eg: td:nth-child(even),th:nth-child(even){
    background-color:pink;
 }
** Vertical & horizontal striping can be combined
Use rgba() color

#Horizontal Dividers
If we want borders only in rows the we use border-bottom property to all tr tag
Eg:tr{
    border-bottom:1px solid black;
}

#Hoverable Table
Using the :hover on tr tag
Eg: tr:hover {background-color:yellow;}

#Colgroup
Used to style specific column
It is written after table tag
Eg:
<colgroup>
<col span="2" style="background-color:pink;"></colgroup>
**empty colgroups
Add "empty" col elements that represents the columns before the columns you want to style
Eg:<colgroup>
<col span="3">
</colgroup>