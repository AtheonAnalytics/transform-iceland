# Location Input

## Transformation Procedure

### 1. Get distinct depot names

Using the **Weekly Depot Stock File**, create a list of distinct values from the _Depot Name_ column.

### 2. Populate table with values

Construct the following table structure populated with the depot name list records and supporting information:

<table><thead><tr><th>Column Name</th><th data-type="select">Source</th><th data-type="select" data-multiple>Source File</th><th>Contents</th></tr></thead><tbody><tr><td>origin_organisation_number</td><td></td><td></td><td>Identifier of the organisation that owns the destination DSR</td></tr><tr><td>business_organisation_number</td><td></td><td></td><td>Identifier of the Retailer organisation</td></tr><tr><td>organisation_location_id</td><td></td><td></td><td>Distinct records from <em>Depot Name</em> column</td></tr><tr><td>location_function</td><td></td><td></td><td>"distribution location"</td></tr><tr><td>geographic_location</td><td></td><td></td><td>NULL</td></tr><tr><td>attributes</td><td></td><td></td><td>JSON object containing key = 'depot_name' and value = distinct records from <em>Depot Name</em> column</td></tr><tr><td>created_timestamp</td><td></td><td></td><td>Timestamp of Source report receipt/creation</td></tr></tbody></table>

{% hint style="info" %}
Source Iceland reports do not provide depot codes, hence the population of _organisation\_location\_id_ with the depot name as the universal identifier
{% endhint %}

### 3. Create DSR Input

Save the transformed data as a file of CSV type with UTF-8 encoding.

## DSR Input Attributes

| Aspect           | Attribute                   |
| ---------------- | --------------------------- |
| Columns          | 7                           |
| Rows             | <7                          |
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
