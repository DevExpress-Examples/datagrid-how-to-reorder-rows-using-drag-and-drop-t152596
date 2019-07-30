<!-- default file list -->
*Files to look at*:

<!-- default file list end -->
# DataGrid  - How to reorder rows using drag-and-drop
<!-- run online -->
**[[Run Online]](https://codecentral.devexpress.com/t152596/)**
<!-- run online end -->


This example demonstrates how to move <a href="http://js.devexpress.com/Documentation/ApiReference/UI_Widgets/dxDataGrid/?version=14_1">dxDataGrid</a> rows using <a href="http://jqueryui.com/draggable/">Draggable</a> and <a href="http://jqueryui.com/droppable/">Droppable</a> plug-ins of the jQueryUI library. <br><br>To accomplish this task, we need to perform the following steps:<br><br>1. Set a fake CSS class ("myRow") to a data row. This will help us find all data rows using a jQuery selector and assign Draggable and Droppable plug-ins to the rows. Assign the key value of each row to a row element. We need to use the <a href="http://js.devexpress.com/Documentation/ApiReference/UI_Widgets/dxDataGrid/Configuration/?version=14_1#rowPrepared">dxDataGrid.rowPrepared</a> callback function for this step.<br>2. When the <a href="http://api.jqueryui.com/droppable/#event-drop">drop</a> event fires, we need to get indexes of the dropped and the target rows, recalculate indexes according our requirements and save them to a data store.<br>3. Reload data by calling the <a href="http://js.devexpress.com/Documentation/ApiReference/UI_Widgets/dxDataGrid/Methods/?version=14_1#refresh">dxDataGrid.refresh</a> method.<br><br><strong>See also:</strong><br><a href="http://js.devexpress.com/Documentation/ApiReference/Data_Library/ArrayStore/Methods/?version=14_1#loadoptions">ArrayStore.load</a> <br><a href="http://js.devexpress.com/Documentation/ApiReference/Data_Library/ArrayStore/Methods/?version=14_1#byKeykey_extraOptions">ArrayStore.byKey</a> <br><a href="http://js.devexpress.com/Documentation/ApiReference/Data_Library/ArrayStore/Methods/?version=14_1#updatekey_values">ArrayStore.update</a> <br><a href="http://api.jquery.com/data/">.data()</a>

<br/>


