# act\_mvt\_weeksku Input

## Transformation Procedure

### 1. Retrieve data

Join the **Weekly Sales File** to the **Weekly Estate Stock File** at the level of detail of both files, allowing data to remain in the absence of a joined record.

Pass all data rows through without amendment into the appropriate columns.

### 2. Populate table with values

<table><thead><tr><th>Column Name</th><th data-type="select">Source</th><th data-type="select" data-multiple>Source File</th><th>Contents</th></tr></thead><tbody><tr><td>organisation_week_id</td><td></td><td></td><td></td></tr><tr><td>organisation_year_id</td><td></td><td></td><td></td></tr><tr><td>source_db_id</td><td></td><td></td><td>Identifier of the Retailer organisation</td></tr><tr><td>organisation_sku</td><td></td><td></td><td><em>Variant SKU</em></td></tr><tr><td>epos_eaches</td><td></td><td></td><td><em>Sales Units</em></td></tr><tr><td>epos_value</td><td></td><td></td><td><em>Sales Turnover</em></td></tr><tr><td>epos_value_net_vat</td><td></td><td></td><td>NULL</td></tr><tr><td>rtc_epos_eaches</td><td></td><td></td><td>NULL</td></tr><tr><td>rtc_epos_value</td><td></td><td></td><td>NULL</td></tr><tr><td>rtc_reduction_value</td><td></td><td></td><td>NULL</td></tr><tr><td>bin_waste_eaches</td><td></td><td></td><td>NULL</td></tr><tr><td>bin_waste_value</td><td></td><td></td><td>NULL</td></tr><tr><td>total_waste_eaches</td><td></td><td></td><td><em>Shrinkage Units</em></td></tr><tr><td>total_waste_value</td><td></td><td></td><td><em>Shrinkage Value</em></td></tr><tr><td>lost_sales_eaches</td><td></td><td></td><td>NULL</td></tr><tr><td>lost_sales_value</td><td></td><td></td><td>NULL</td></tr><tr><td>organisation_service_level_percentage</td><td></td><td></td><td></td></tr><tr><td>depot_cases_ordered_out</td><td></td><td></td><td>NULL</td></tr><tr><td>depot_cases_fulfilled_out</td><td></td><td></td><td><em>Delivered Cases Store</em></td></tr><tr><td>depot_units_ordered_out</td><td></td><td></td><td>NULL</td></tr><tr><td>depot_units_fulfilled_out</td><td></td><td></td><td>= <em>Delivered Cases Store</em> x <em>Retail Units</em></td></tr><tr><td>created_timestamp</td><td></td><td></td><td></td></tr><tr><td>submitting_business_organisation_number</td><td></td><td></td><td>Identifier of the organisation that is submitting the data to the destination DSR</td></tr><tr><td>primary_subject_business_organisation_number</td><td></td><td></td><td><em>Supplier Number</em></td></tr><tr><td>primary_subject_origin_organisation_number</td><td></td><td></td><td>Identifier of the Retailer organisation</td></tr></tbody></table>

### 3. Create DSR Input

Save the transformed data as a file of CSV type with UTF-8 encoding.

## DSR Input Attributes

| Aspect           | Attribute                   |
| ---------------- | --------------------------- |
| Columns          | 25                          |
| Rows             | <\~500                      |
| Header Row       | Yes                         |
| Data Protocol    | File                        |
| File Type        | CSV                         |
| Encoding         | UTF-8                       |
| Timestamp Format | YYYY-MM-DD HH:MI:SS TZH:TZM |

## Test Regime

| Test | Expected Output |
| ---- | --------------- |
|      |                 |
|      |                 |
|      |                 |

## Example DSR Input

{% content-ref url="example-dsr-input.md" %}
[example-dsr-input.md](example-dsr-input.md)
{% endcontent-ref %}
