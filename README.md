# How to apply row hover background color in .NET MAUI DataGrid?

This article demonstrates how to apply row hover background color in [.NET MAUI DataGrid](https://www.syncfusion.com/maui-controls/maui-datagrid).

In SfDataGrid, the row hover highlighting effect can be enabled by configuring the [AllowRowHoverHighlighting](https://help.syncfusion.com/cr/maui/Syncfusion.Maui.DataGrid.SfDataGrid.html#Syncfusion_Maui_DataGrid_SfDataGrid_AllowRowHoverHighlighting) property to true.. To customize the background color when a row is hovered, use the [RowHoveredBackground](https://help.syncfusion.com/cr/maui/Syncfusion.Maui.DataGrid.DataGridStyle.html#Syncfusion_Maui_DataGrid_DataGridStyle_RowHoveredBackground) property within the [SfDataGrid.DefaultStyle](https://help.syncfusion.com/cr/maui/Syncfusion.Maui.DataGrid.SfDataGrid.html#Syncfusion_Maui_DataGrid_SfDataGrid_DefaultStyleProperty). This ensures that the specified color is applied to the row when the mouse hovers over it.

## XAML

```xml
<ContentPage xmlns:syncfusion="http://schemas.syncfusion.com/maui">
    <ContentPage.Content>
        <syncfusion:SfDataGrid x:Name="dataGrid"
                               ItemsSource="{Binding OrderInfoCollection}"
                               AllowRowHoverHighlighting="True">
            <syncfusion:SfDataGrid.DefaultStyle>
                <syncfusion:DataGridStyle RowHoveredBackground ="#AFD5FB"/>
            </syncfusion:SfDataGrid.DefaultStyle>
        </syncfusion:SfDataGrid>
    </ContentPage.Content>
</ContentPage>
```

Download the complete sample from [GitHub](https://github.com/SyncfusionExamples/How-to-apply-row-hover-background-color-in-.NET-MAUI-DataGrid)