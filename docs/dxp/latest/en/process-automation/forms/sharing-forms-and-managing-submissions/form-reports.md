# Form Reports

> Available: Liferay CE/DXP 7.3

Once users begin submitting form entries, you can access a field-by-field report on the form's records:

1. Navigate to the Forms application. In the Product Menu (![Product Menu](../../../images/icon-product-menu.png)), go to _Content & Data_ &rarr; _Forms_.

1. Click the form's _Name_ to open the form builder view.

1. Click the _Entries_ tab. The first datum presented is the count of all entries currently submitted.

   ![The number of submitted entries is displayed at the top of the Entries screen.](./form-reports/images/06.png)

   Field-by-field metrics are presented next. Scroll through the fields or click a specific field from the list on the right to jump to its metrics.

   ![This Rate It Select from List field has received mostly "Good" selections.](./form-reports/images/01.png)

```{tip}
Form Reports shows you aggregated form data. To see each form entry individually, see [Managing Form Entries](./managing-form-entries.md#viewing-form-entries).
```

## Form Fields and Chart Types

The data presentation is different depending on the field type:

| Field(s) | Data Display Format | Additional Information |
| -------- | ---------- | ---------------------- |
| Color<br />Date<br />Number<br />Text| Field List | Number fields also include these summary statistics: Average, Maximum Value, Minimum Value, Sum |
| Select from List<br />Single Selection | Pie Chart | None |
| Grid<br />Multiple Selection | Bar Graph | Multiple Selection graphs are horizontal, where Grid graphs are vertical with grouped bars
| Image<br />Paragraph<br />Rich Text<br />Separator<br />Upload | _No Metrics_ | These fields don't have metrics to report |

### Field Lists

The Color, Date, Number, and Text fields accept free-form data entry from the form's users, so data can't really be tabulated for these fields. Instead, they're presented as a simple list of responses. However, since the number field includes validation to ensure that only numeric data are entered, some summary statistics are compiled: average, sum, minimum value, and maximum value.

![Color field entries are displayed as a simple list of responses.](./form-reports/images/02.png)

### Pie Charts

The Select from List and Single Selection fields accept only one entry selected from a list of choices. A pie chart is displayed to show the proportion of users' selections.

![Single Selection entries are displayed in a pie chart.](./form-reports/images/03.png)

### Bar Graphs

The Multiple Selection field accepts multiple entries for one selection request (e.g., _Select the toppings for your sandwich_). The proportion of selections is displayed in a horizontal bar graph. 

![Multiple Selection entries are displayed in a horizontal bar graph.](./form-reports/images/04.png)

The Grid field accepts a single entry for each of multiple related questions (e.g., _Rate these Sylvester Stallone movies as Good, Bad, or No Opinion_). The proportion of selections is displayed in a vertical bar graph, with bars grouped by question.

![Grid entries are displayed in a vertical bar graph.](./form-reports/images/05.png)

## Related Topics

* [Viewing Form Entries](./managing-form-entries.md#viewing-form-entries)
* [Exporting Form Entries](./managing-form-entries.md#exporting-form-entries)
* [Editing Form Entries](./managing-form-entries.md#editing-form-entries)
