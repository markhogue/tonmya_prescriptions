Tonmya Prescriptions
================
2026-03-22

## Some simple models based on Tonmya sales

What are we doing here? - Just trying to get a grasp on the rate of
increase and projecting out if that rate continues. It is not
necessarily realistic to take it out as far as projections provide.
Nothing here should be regarded as investment advice. I am not a
financial analyst or advisor.

## Sales Projection - at weekly growth rate - *exponential model*

    ## 
    ## Formula: sales ~ a * (1 + r)^wk
    ## 
    ## Parameters:
    ##   Estimate Std. Error t value Pr(>|t|)    
    ## a 73.67419   11.41571   6.454 1.09e-05 ***
    ## r  0.14956    0.01237  12.090 3.90e-09 ***
    ## ---
    ## Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1
    ## 
    ## Residual standard error: 54.68 on 15 degrees of freedom
    ## 
    ## Number of iterations to convergence: 11 
    ## Achieved convergence tolerance: 4.596e-06

The exponential model projects weekly increases of {r
paste0(summary(mod_sales_exp)\$coefficients\[2\] \* 100, ” %“)}

<div id="gibdmztjsu" style="padding-left:0px;padding-right:0px;padding-top:10px;padding-bottom:10px;overflow-x:auto;overflow-y:auto;width:auto;height:auto;">
<style>#gibdmztjsu table {
  font-family: system-ui, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol', 'Noto Color Emoji';
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
&#10;#gibdmztjsu thead, #gibdmztjsu tbody, #gibdmztjsu tfoot, #gibdmztjsu tr, #gibdmztjsu td, #gibdmztjsu th {
  border-style: none;
}
&#10;#gibdmztjsu p {
  margin: 0;
  padding: 0;
}
&#10;#gibdmztjsu .gt_table {
  display: table;
  border-collapse: collapse;
  line-height: normal;
  margin-left: auto;
  margin-right: auto;
  color: #333333;
  font-size: 16px;
  font-weight: normal;
  font-style: normal;
  background-color: #FFFFFF;
  width: auto;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #A8A8A8;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #A8A8A8;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
}
&#10;#gibdmztjsu .gt_caption {
  padding-top: 4px;
  padding-bottom: 4px;
}
&#10;#gibdmztjsu .gt_title {
  color: #333333;
  font-size: 125%;
  font-weight: initial;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-color: #FFFFFF;
  border-bottom-width: 0;
}
&#10;#gibdmztjsu .gt_subtitle {
  color: #333333;
  font-size: 85%;
  font-weight: initial;
  padding-top: 3px;
  padding-bottom: 5px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-color: #FFFFFF;
  border-top-width: 0;
}
&#10;#gibdmztjsu .gt_heading {
  background-color: #FFFFFF;
  text-align: center;
  border-bottom-color: #FFFFFF;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}
&#10;#gibdmztjsu .gt_bottom_border {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}
&#10;#gibdmztjsu .gt_col_headings {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}
&#10;#gibdmztjsu .gt_col_heading {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 6px;
  padding-left: 5px;
  padding-right: 5px;
  overflow-x: hidden;
}
&#10;#gibdmztjsu .gt_column_spanner_outer {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  padding-top: 0;
  padding-bottom: 0;
  padding-left: 4px;
  padding-right: 4px;
}
&#10;#gibdmztjsu .gt_column_spanner_outer:first-child {
  padding-left: 0;
}
&#10;#gibdmztjsu .gt_column_spanner_outer:last-child {
  padding-right: 0;
}
&#10;#gibdmztjsu .gt_column_spanner {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 5px;
  overflow-x: hidden;
  display: inline-block;
  width: 100%;
}
&#10;#gibdmztjsu .gt_spanner_row {
  border-bottom-style: hidden;
}
&#10;#gibdmztjsu .gt_group_heading {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  text-align: left;
}
&#10;#gibdmztjsu .gt_empty_group_heading {
  padding: 0.5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: middle;
}
&#10;#gibdmztjsu .gt_from_md > :first-child {
  margin-top: 0;
}
&#10;#gibdmztjsu .gt_from_md > :last-child {
  margin-bottom: 0;
}
&#10;#gibdmztjsu .gt_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  margin: 10px;
  border-top-style: solid;
  border-top-width: 1px;
  border-top-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  overflow-x: hidden;
}
&#10;#gibdmztjsu .gt_stub {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 5px;
  padding-right: 5px;
}
&#10;#gibdmztjsu .gt_stub_row_group {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 5px;
  padding-right: 5px;
  vertical-align: top;
}
&#10;#gibdmztjsu .gt_row_group_first td {
  border-top-width: 2px;
}
&#10;#gibdmztjsu .gt_row_group_first th {
  border-top-width: 2px;
}
&#10;#gibdmztjsu .gt_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}
&#10;#gibdmztjsu .gt_first_summary_row {
  border-top-style: solid;
  border-top-color: #D3D3D3;
}
&#10;#gibdmztjsu .gt_first_summary_row.thick {
  border-top-width: 2px;
}
&#10;#gibdmztjsu .gt_last_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}
&#10;#gibdmztjsu .gt_grand_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}
&#10;#gibdmztjsu .gt_first_grand_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-style: double;
  border-top-width: 6px;
  border-top-color: #D3D3D3;
}
&#10;#gibdmztjsu .gt_last_grand_summary_row_top {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-style: double;
  border-bottom-width: 6px;
  border-bottom-color: #D3D3D3;
}
&#10;#gibdmztjsu .gt_striped {
  background-color: rgba(128, 128, 128, 0.05);
}
&#10;#gibdmztjsu .gt_table_body {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}
&#10;#gibdmztjsu .gt_footnotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}
&#10;#gibdmztjsu .gt_footnote {
  margin: 0px;
  font-size: 90%;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
}
&#10;#gibdmztjsu .gt_sourcenotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}
&#10;#gibdmztjsu .gt_sourcenote {
  font-size: 90%;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
}
&#10;#gibdmztjsu .gt_left {
  text-align: left;
}
&#10;#gibdmztjsu .gt_center {
  text-align: center;
}
&#10;#gibdmztjsu .gt_right {
  text-align: right;
  font-variant-numeric: tabular-nums;
}
&#10;#gibdmztjsu .gt_font_normal {
  font-weight: normal;
}
&#10;#gibdmztjsu .gt_font_bold {
  font-weight: bold;
}
&#10;#gibdmztjsu .gt_font_italic {
  font-style: italic;
}
&#10;#gibdmztjsu .gt_super {
  font-size: 65%;
}
&#10;#gibdmztjsu .gt_footnote_marks {
  font-size: 75%;
  vertical-align: 0.4em;
  position: initial;
}
&#10;#gibdmztjsu .gt_asterisk {
  font-size: 100%;
  vertical-align: 0;
}
&#10;#gibdmztjsu .gt_indent_1 {
  text-indent: 5px;
}
&#10;#gibdmztjsu .gt_indent_2 {
  text-indent: 10px;
}
&#10;#gibdmztjsu .gt_indent_3 {
  text-indent: 15px;
}
&#10;#gibdmztjsu .gt_indent_4 {
  text-indent: 20px;
}
&#10;#gibdmztjsu .gt_indent_5 {
  text-indent: 25px;
}
&#10;#gibdmztjsu .katex-display {
  display: inline-flex !important;
  margin-bottom: 0.75em !important;
}
&#10;#gibdmztjsu div.Reactable > div.rt-table > div.rt-thead > div.rt-tr.rt-tr-group-header > div.rt-th-group:after {
  height: 0px !important;
}
</style>
<table class="gt_table" data-quarto-disable-processing="false" data-quarto-bootstrap="false">
  <thead>
    <tr class="gt_heading">
      <td colspan="4" class="gt_heading gt_title gt_font_normal gt_bottom_border" style><span class='gt_from_md'>Exponential Model</span></td>
    </tr>
    &#10;    <tr class="gt_col_headings">
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="wk">wk</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="sales_reported">sales_reported</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="exponential_model">exponential_model</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="yearly_rate_predicted_M">yearly_rate_predicted_M</th>
    </tr>
  </thead>
  <tbody class="gt_table_body">
    <tr><td headers="wk" class="gt_row gt_right">1</td>
<td headers="sales_reported" class="gt_row gt_right">2</td>
<td headers="exponential_model" class="gt_row gt_right">85</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">4.4</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">2</td>
<td headers="sales_reported" class="gt_row gt_right">16</td>
<td headers="exponential_model" class="gt_row gt_right">97</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">5.1</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">3</td>
<td headers="sales_reported" class="gt_row gt_right">54</td>
<td headers="exponential_model" class="gt_row gt_right">112</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">5.8</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">4</td>
<td headers="sales_reported" class="gt_row gt_right">93</td>
<td headers="exponential_model" class="gt_row gt_right">129</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">6.7</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">5</td>
<td headers="sales_reported" class="gt_row gt_right">179</td>
<td headers="exponential_model" class="gt_row gt_right">148</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">7.7</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">6</td>
<td headers="sales_reported" class="gt_row gt_right">268</td>
<td headers="exponential_model" class="gt_row gt_right">170</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">8.8</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">7</td>
<td headers="sales_reported" class="gt_row gt_right">212</td>
<td headers="exponential_model" class="gt_row gt_right">195</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">10.2</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">8</td>
<td headers="sales_reported" class="gt_row gt_right">187</td>
<td headers="exponential_model" class="gt_row gt_right">225</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">11.7</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">9</td>
<td headers="sales_reported" class="gt_row gt_right">264</td>
<td headers="exponential_model" class="gt_row gt_right">258</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">13.4</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">10</td>
<td headers="sales_reported" class="gt_row gt_right">324</td>
<td headers="exponential_model" class="gt_row gt_right">297</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">15.4</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">11</td>
<td headers="sales_reported" class="gt_row gt_right">367</td>
<td headers="exponential_model" class="gt_row gt_right">341</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">17.7</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">12</td>
<td headers="sales_reported" class="gt_row gt_right">352</td>
<td headers="exponential_model" class="gt_row gt_right">392</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">20.4</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">13</td>
<td headers="sales_reported" class="gt_row gt_right">451</td>
<td headers="exponential_model" class="gt_row gt_right">451</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">23.5</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">14</td>
<td headers="sales_reported" class="gt_row gt_right">598</td>
<td headers="exponential_model" class="gt_row gt_right">519</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">27.0</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">15</td>
<td headers="sales_reported" class="gt_row gt_right">639</td>
<td headers="exponential_model" class="gt_row gt_right">596</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">31.0</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">16</td>
<td headers="sales_reported" class="gt_row gt_right">642</td>
<td headers="exponential_model" class="gt_row gt_right">685</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">35.6</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">17</td>
<td headers="sales_reported" class="gt_row gt_right">750</td>
<td headers="exponential_model" class="gt_row gt_right">788</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">41.0</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">18</td>
<td headers="sales_reported" class="gt_row gt_right">NA</td>
<td headers="exponential_model" class="gt_row gt_right">905</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">47.1</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">19</td>
<td headers="sales_reported" class="gt_row gt_right">NA</td>
<td headers="exponential_model" class="gt_row gt_right">1041</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">54.1</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">20</td>
<td headers="sales_reported" class="gt_row gt_right">NA</td>
<td headers="exponential_model" class="gt_row gt_right">1197</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">62.2</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">21</td>
<td headers="sales_reported" class="gt_row gt_right">NA</td>
<td headers="exponential_model" class="gt_row gt_right">1376</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">71.5</td></tr>
  </tbody>
  &#10;</table>
</div>

![](Tonmya_prescriptions_files/figure-gfm/sales%20exponential%202-1.png)<!-- -->
\## Sales Projection - at weekly rate - *linear model*

    ## 
    ## Call:
    ## lm(formula = sales ~ wk, data = df_sales)
    ## 
    ## Residuals:
    ##     Min      1Q  Median      3Q     Max 
    ## -99.265 -39.686   3.941  41.098  84.206 
    ## 
    ## Coefficients:
    ##             Estimate Std. Error t value Pr(>|t|)    
    ## (Intercept)  -83.676     28.710  -2.915   0.0107 *  
    ## wk            44.578      2.802  15.911 8.42e-11 ***
    ## ---
    ## Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1
    ## 
    ## Residual standard error: 56.59 on 15 degrees of freedom
    ## Multiple R-squared:  0.9441, Adjusted R-squared:  0.9403 
    ## F-statistic: 253.2 on 1 and 15 DF,  p-value: 8.423e-11

<div id="wwglpxssjv" style="padding-left:0px;padding-right:0px;padding-top:10px;padding-bottom:10px;overflow-x:auto;overflow-y:auto;width:auto;height:auto;">
<style>#wwglpxssjv table {
  font-family: system-ui, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol', 'Noto Color Emoji';
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
&#10;#wwglpxssjv thead, #wwglpxssjv tbody, #wwglpxssjv tfoot, #wwglpxssjv tr, #wwglpxssjv td, #wwglpxssjv th {
  border-style: none;
}
&#10;#wwglpxssjv p {
  margin: 0;
  padding: 0;
}
&#10;#wwglpxssjv .gt_table {
  display: table;
  border-collapse: collapse;
  line-height: normal;
  margin-left: auto;
  margin-right: auto;
  color: #333333;
  font-size: 16px;
  font-weight: normal;
  font-style: normal;
  background-color: #FFFFFF;
  width: auto;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #A8A8A8;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #A8A8A8;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
}
&#10;#wwglpxssjv .gt_caption {
  padding-top: 4px;
  padding-bottom: 4px;
}
&#10;#wwglpxssjv .gt_title {
  color: #333333;
  font-size: 125%;
  font-weight: initial;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-color: #FFFFFF;
  border-bottom-width: 0;
}
&#10;#wwglpxssjv .gt_subtitle {
  color: #333333;
  font-size: 85%;
  font-weight: initial;
  padding-top: 3px;
  padding-bottom: 5px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-color: #FFFFFF;
  border-top-width: 0;
}
&#10;#wwglpxssjv .gt_heading {
  background-color: #FFFFFF;
  text-align: center;
  border-bottom-color: #FFFFFF;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}
&#10;#wwglpxssjv .gt_bottom_border {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}
&#10;#wwglpxssjv .gt_col_headings {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}
&#10;#wwglpxssjv .gt_col_heading {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 6px;
  padding-left: 5px;
  padding-right: 5px;
  overflow-x: hidden;
}
&#10;#wwglpxssjv .gt_column_spanner_outer {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  padding-top: 0;
  padding-bottom: 0;
  padding-left: 4px;
  padding-right: 4px;
}
&#10;#wwglpxssjv .gt_column_spanner_outer:first-child {
  padding-left: 0;
}
&#10;#wwglpxssjv .gt_column_spanner_outer:last-child {
  padding-right: 0;
}
&#10;#wwglpxssjv .gt_column_spanner {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 5px;
  overflow-x: hidden;
  display: inline-block;
  width: 100%;
}
&#10;#wwglpxssjv .gt_spanner_row {
  border-bottom-style: hidden;
}
&#10;#wwglpxssjv .gt_group_heading {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  text-align: left;
}
&#10;#wwglpxssjv .gt_empty_group_heading {
  padding: 0.5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: middle;
}
&#10;#wwglpxssjv .gt_from_md > :first-child {
  margin-top: 0;
}
&#10;#wwglpxssjv .gt_from_md > :last-child {
  margin-bottom: 0;
}
&#10;#wwglpxssjv .gt_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  margin: 10px;
  border-top-style: solid;
  border-top-width: 1px;
  border-top-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  overflow-x: hidden;
}
&#10;#wwglpxssjv .gt_stub {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 5px;
  padding-right: 5px;
}
&#10;#wwglpxssjv .gt_stub_row_group {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 5px;
  padding-right: 5px;
  vertical-align: top;
}
&#10;#wwglpxssjv .gt_row_group_first td {
  border-top-width: 2px;
}
&#10;#wwglpxssjv .gt_row_group_first th {
  border-top-width: 2px;
}
&#10;#wwglpxssjv .gt_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}
&#10;#wwglpxssjv .gt_first_summary_row {
  border-top-style: solid;
  border-top-color: #D3D3D3;
}
&#10;#wwglpxssjv .gt_first_summary_row.thick {
  border-top-width: 2px;
}
&#10;#wwglpxssjv .gt_last_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}
&#10;#wwglpxssjv .gt_grand_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}
&#10;#wwglpxssjv .gt_first_grand_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-style: double;
  border-top-width: 6px;
  border-top-color: #D3D3D3;
}
&#10;#wwglpxssjv .gt_last_grand_summary_row_top {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-style: double;
  border-bottom-width: 6px;
  border-bottom-color: #D3D3D3;
}
&#10;#wwglpxssjv .gt_striped {
  background-color: rgba(128, 128, 128, 0.05);
}
&#10;#wwglpxssjv .gt_table_body {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}
&#10;#wwglpxssjv .gt_footnotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}
&#10;#wwglpxssjv .gt_footnote {
  margin: 0px;
  font-size: 90%;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
}
&#10;#wwglpxssjv .gt_sourcenotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}
&#10;#wwglpxssjv .gt_sourcenote {
  font-size: 90%;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
}
&#10;#wwglpxssjv .gt_left {
  text-align: left;
}
&#10;#wwglpxssjv .gt_center {
  text-align: center;
}
&#10;#wwglpxssjv .gt_right {
  text-align: right;
  font-variant-numeric: tabular-nums;
}
&#10;#wwglpxssjv .gt_font_normal {
  font-weight: normal;
}
&#10;#wwglpxssjv .gt_font_bold {
  font-weight: bold;
}
&#10;#wwglpxssjv .gt_font_italic {
  font-style: italic;
}
&#10;#wwglpxssjv .gt_super {
  font-size: 65%;
}
&#10;#wwglpxssjv .gt_footnote_marks {
  font-size: 75%;
  vertical-align: 0.4em;
  position: initial;
}
&#10;#wwglpxssjv .gt_asterisk {
  font-size: 100%;
  vertical-align: 0;
}
&#10;#wwglpxssjv .gt_indent_1 {
  text-indent: 5px;
}
&#10;#wwglpxssjv .gt_indent_2 {
  text-indent: 10px;
}
&#10;#wwglpxssjv .gt_indent_3 {
  text-indent: 15px;
}
&#10;#wwglpxssjv .gt_indent_4 {
  text-indent: 20px;
}
&#10;#wwglpxssjv .gt_indent_5 {
  text-indent: 25px;
}
&#10;#wwglpxssjv .katex-display {
  display: inline-flex !important;
  margin-bottom: 0.75em !important;
}
&#10;#wwglpxssjv div.Reactable > div.rt-table > div.rt-thead > div.rt-tr.rt-tr-group-header > div.rt-th-group:after {
  height: 0px !important;
}
</style>
<table class="gt_table" data-quarto-disable-processing="false" data-quarto-bootstrap="false">
  <thead>
    <tr class="gt_heading">
      <td colspan="4" class="gt_heading gt_title gt_font_normal gt_bottom_border" style><span class='gt_from_md'>Linear Model</span></td>
    </tr>
    &#10;    <tr class="gt_col_headings">
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="wk">wk</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="sales_reported">sales_reported</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="linear_model">linear_model</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="yearly_rate_predicted_M">yearly_rate_predicted_M</th>
    </tr>
  </thead>
  <tbody class="gt_table_body">
    <tr><td headers="wk" class="gt_row gt_right">1</td>
<td headers="sales_reported" class="gt_row gt_right">2</td>
<td headers="linear_model" class="gt_row gt_right">44.6</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">2.3</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">2</td>
<td headers="sales_reported" class="gt_row gt_right">16</td>
<td headers="linear_model" class="gt_row gt_right">89.2</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">4.6</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">3</td>
<td headers="sales_reported" class="gt_row gt_right">54</td>
<td headers="linear_model" class="gt_row gt_right">133.7</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">7.0</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">4</td>
<td headers="sales_reported" class="gt_row gt_right">93</td>
<td headers="linear_model" class="gt_row gt_right">178.3</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">9.3</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">5</td>
<td headers="sales_reported" class="gt_row gt_right">179</td>
<td headers="linear_model" class="gt_row gt_right">222.9</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">11.6</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">6</td>
<td headers="sales_reported" class="gt_row gt_right">268</td>
<td headers="linear_model" class="gt_row gt_right">267.5</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">13.9</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">7</td>
<td headers="sales_reported" class="gt_row gt_right">212</td>
<td headers="linear_model" class="gt_row gt_right">312.0</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">16.2</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">8</td>
<td headers="sales_reported" class="gt_row gt_right">187</td>
<td headers="linear_model" class="gt_row gt_right">356.6</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">18.5</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">9</td>
<td headers="sales_reported" class="gt_row gt_right">264</td>
<td headers="linear_model" class="gt_row gt_right">401.2</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">20.9</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">10</td>
<td headers="sales_reported" class="gt_row gt_right">324</td>
<td headers="linear_model" class="gt_row gt_right">445.8</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">23.2</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">11</td>
<td headers="sales_reported" class="gt_row gt_right">367</td>
<td headers="linear_model" class="gt_row gt_right">490.4</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">25.5</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">12</td>
<td headers="sales_reported" class="gt_row gt_right">352</td>
<td headers="linear_model" class="gt_row gt_right">534.9</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">27.8</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">13</td>
<td headers="sales_reported" class="gt_row gt_right">451</td>
<td headers="linear_model" class="gt_row gt_right">579.5</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">30.1</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">14</td>
<td headers="sales_reported" class="gt_row gt_right">598</td>
<td headers="linear_model" class="gt_row gt_right">624.1</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">32.5</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">15</td>
<td headers="sales_reported" class="gt_row gt_right">639</td>
<td headers="linear_model" class="gt_row gt_right">668.7</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">34.8</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">16</td>
<td headers="sales_reported" class="gt_row gt_right">642</td>
<td headers="linear_model" class="gt_row gt_right">713.3</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">37.1</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">17</td>
<td headers="sales_reported" class="gt_row gt_right">750</td>
<td headers="linear_model" class="gt_row gt_right">757.8</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">39.4</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">18</td>
<td headers="sales_reported" class="gt_row gt_right">NA</td>
<td headers="linear_model" class="gt_row gt_right">802.4</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">41.7</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">19</td>
<td headers="sales_reported" class="gt_row gt_right">NA</td>
<td headers="linear_model" class="gt_row gt_right">847.0</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">44.0</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">20</td>
<td headers="sales_reported" class="gt_row gt_right">NA</td>
<td headers="linear_model" class="gt_row gt_right">891.6</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">46.4</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">21</td>
<td headers="sales_reported" class="gt_row gt_right">NA</td>
<td headers="linear_model" class="gt_row gt_right">936.1</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">48.7</td></tr>
  </tbody>
  &#10;</table>
</div>

![](Tonmya_prescriptions_files/figure-gfm/sales%20linear-1.png)<!-- -->

## scripts Projection - at weekly growth rate - *exponential model*

    ## 
    ## Formula: scripts ~ a * (1 + r)^wk
    ## 
    ## Parameters:
    ##   Estimate Std. Error t value Pr(>|t|)    
    ## a 44.34214    6.83615   6.486 1.03e-05 ***
    ## r  0.15107    0.01231  12.276 3.16e-09 ***
    ## ---
    ## Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1
    ## 
    ## Residual standard error: 33.1 on 15 degrees of freedom
    ## 
    ## Number of iterations to convergence: 8 
    ## Achieved convergence tolerance: 1.286e-06

The exponential model projects weekly increases of {r
paste0(summary(mod_scripts_exp)\$coefficients\[2\] \* 100, ” %“)}

<div id="mzqojzeefo" style="padding-left:0px;padding-right:0px;padding-top:10px;padding-bottom:10px;overflow-x:auto;overflow-y:auto;width:auto;height:auto;">
<style>#mzqojzeefo table {
  font-family: system-ui, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol', 'Noto Color Emoji';
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
&#10;#mzqojzeefo thead, #mzqojzeefo tbody, #mzqojzeefo tfoot, #mzqojzeefo tr, #mzqojzeefo td, #mzqojzeefo th {
  border-style: none;
}
&#10;#mzqojzeefo p {
  margin: 0;
  padding: 0;
}
&#10;#mzqojzeefo .gt_table {
  display: table;
  border-collapse: collapse;
  line-height: normal;
  margin-left: auto;
  margin-right: auto;
  color: #333333;
  font-size: 16px;
  font-weight: normal;
  font-style: normal;
  background-color: #FFFFFF;
  width: auto;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #A8A8A8;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #A8A8A8;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
}
&#10;#mzqojzeefo .gt_caption {
  padding-top: 4px;
  padding-bottom: 4px;
}
&#10;#mzqojzeefo .gt_title {
  color: #333333;
  font-size: 125%;
  font-weight: initial;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-color: #FFFFFF;
  border-bottom-width: 0;
}
&#10;#mzqojzeefo .gt_subtitle {
  color: #333333;
  font-size: 85%;
  font-weight: initial;
  padding-top: 3px;
  padding-bottom: 5px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-color: #FFFFFF;
  border-top-width: 0;
}
&#10;#mzqojzeefo .gt_heading {
  background-color: #FFFFFF;
  text-align: center;
  border-bottom-color: #FFFFFF;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}
&#10;#mzqojzeefo .gt_bottom_border {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}
&#10;#mzqojzeefo .gt_col_headings {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}
&#10;#mzqojzeefo .gt_col_heading {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 6px;
  padding-left: 5px;
  padding-right: 5px;
  overflow-x: hidden;
}
&#10;#mzqojzeefo .gt_column_spanner_outer {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  padding-top: 0;
  padding-bottom: 0;
  padding-left: 4px;
  padding-right: 4px;
}
&#10;#mzqojzeefo .gt_column_spanner_outer:first-child {
  padding-left: 0;
}
&#10;#mzqojzeefo .gt_column_spanner_outer:last-child {
  padding-right: 0;
}
&#10;#mzqojzeefo .gt_column_spanner {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 5px;
  overflow-x: hidden;
  display: inline-block;
  width: 100%;
}
&#10;#mzqojzeefo .gt_spanner_row {
  border-bottom-style: hidden;
}
&#10;#mzqojzeefo .gt_group_heading {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  text-align: left;
}
&#10;#mzqojzeefo .gt_empty_group_heading {
  padding: 0.5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: middle;
}
&#10;#mzqojzeefo .gt_from_md > :first-child {
  margin-top: 0;
}
&#10;#mzqojzeefo .gt_from_md > :last-child {
  margin-bottom: 0;
}
&#10;#mzqojzeefo .gt_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  margin: 10px;
  border-top-style: solid;
  border-top-width: 1px;
  border-top-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  overflow-x: hidden;
}
&#10;#mzqojzeefo .gt_stub {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 5px;
  padding-right: 5px;
}
&#10;#mzqojzeefo .gt_stub_row_group {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 5px;
  padding-right: 5px;
  vertical-align: top;
}
&#10;#mzqojzeefo .gt_row_group_first td {
  border-top-width: 2px;
}
&#10;#mzqojzeefo .gt_row_group_first th {
  border-top-width: 2px;
}
&#10;#mzqojzeefo .gt_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}
&#10;#mzqojzeefo .gt_first_summary_row {
  border-top-style: solid;
  border-top-color: #D3D3D3;
}
&#10;#mzqojzeefo .gt_first_summary_row.thick {
  border-top-width: 2px;
}
&#10;#mzqojzeefo .gt_last_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}
&#10;#mzqojzeefo .gt_grand_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}
&#10;#mzqojzeefo .gt_first_grand_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-style: double;
  border-top-width: 6px;
  border-top-color: #D3D3D3;
}
&#10;#mzqojzeefo .gt_last_grand_summary_row_top {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-style: double;
  border-bottom-width: 6px;
  border-bottom-color: #D3D3D3;
}
&#10;#mzqojzeefo .gt_striped {
  background-color: rgba(128, 128, 128, 0.05);
}
&#10;#mzqojzeefo .gt_table_body {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}
&#10;#mzqojzeefo .gt_footnotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}
&#10;#mzqojzeefo .gt_footnote {
  margin: 0px;
  font-size: 90%;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
}
&#10;#mzqojzeefo .gt_sourcenotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}
&#10;#mzqojzeefo .gt_sourcenote {
  font-size: 90%;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
}
&#10;#mzqojzeefo .gt_left {
  text-align: left;
}
&#10;#mzqojzeefo .gt_center {
  text-align: center;
}
&#10;#mzqojzeefo .gt_right {
  text-align: right;
  font-variant-numeric: tabular-nums;
}
&#10;#mzqojzeefo .gt_font_normal {
  font-weight: normal;
}
&#10;#mzqojzeefo .gt_font_bold {
  font-weight: bold;
}
&#10;#mzqojzeefo .gt_font_italic {
  font-style: italic;
}
&#10;#mzqojzeefo .gt_super {
  font-size: 65%;
}
&#10;#mzqojzeefo .gt_footnote_marks {
  font-size: 75%;
  vertical-align: 0.4em;
  position: initial;
}
&#10;#mzqojzeefo .gt_asterisk {
  font-size: 100%;
  vertical-align: 0;
}
&#10;#mzqojzeefo .gt_indent_1 {
  text-indent: 5px;
}
&#10;#mzqojzeefo .gt_indent_2 {
  text-indent: 10px;
}
&#10;#mzqojzeefo .gt_indent_3 {
  text-indent: 15px;
}
&#10;#mzqojzeefo .gt_indent_4 {
  text-indent: 20px;
}
&#10;#mzqojzeefo .gt_indent_5 {
  text-indent: 25px;
}
&#10;#mzqojzeefo .katex-display {
  display: inline-flex !important;
  margin-bottom: 0.75em !important;
}
&#10;#mzqojzeefo div.Reactable > div.rt-table > div.rt-thead > div.rt-tr.rt-tr-group-header > div.rt-th-group:after {
  height: 0px !important;
}
</style>
<table class="gt_table" data-quarto-disable-processing="false" data-quarto-bootstrap="false">
  <thead>
    <tr class="gt_heading">
      <td colspan="4" class="gt_heading gt_title gt_font_normal gt_bottom_border" style><span class='gt_from_md'>Exponential Model</span></td>
    </tr>
    &#10;    <tr class="gt_col_headings">
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="wk">wk</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="scripts_reported">scripts_reported</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="exponential_model">exponential_model</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="yearly_rate_predicted_M">yearly_rate_predicted_M</th>
    </tr>
  </thead>
  <tbody class="gt_table_body">
    <tr><td headers="wk" class="gt_row gt_right">1</td>
<td headers="scripts_reported" class="gt_row gt_right">2</td>
<td headers="exponential_model" class="gt_row gt_right">51</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">2.7</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">2</td>
<td headers="scripts_reported" class="gt_row gt_right">12</td>
<td headers="exponential_model" class="gt_row gt_right">59</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">3.1</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">3</td>
<td headers="scripts_reported" class="gt_row gt_right">35</td>
<td headers="exponential_model" class="gt_row gt_right">68</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">3.5</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">4</td>
<td headers="scripts_reported" class="gt_row gt_right">60</td>
<td headers="exponential_model" class="gt_row gt_right">78</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">4.0</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">5</td>
<td headers="scripts_reported" class="gt_row gt_right">126</td>
<td headers="exponential_model" class="gt_row gt_right">90</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">4.7</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">6</td>
<td headers="scripts_reported" class="gt_row gt_right">154</td>
<td headers="exponential_model" class="gt_row gt_right">103</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">5.4</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">7</td>
<td headers="scripts_reported" class="gt_row gt_right">127</td>
<td headers="exponential_model" class="gt_row gt_right">119</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">6.2</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">8</td>
<td headers="scripts_reported" class="gt_row gt_right">108</td>
<td headers="exponential_model" class="gt_row gt_right">137</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">7.1</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">9</td>
<td headers="scripts_reported" class="gt_row gt_right">163</td>
<td headers="exponential_model" class="gt_row gt_right">157</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">8.2</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">10</td>
<td headers="scripts_reported" class="gt_row gt_right">193</td>
<td headers="exponential_model" class="gt_row gt_right">181</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">9.4</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">11</td>
<td headers="scripts_reported" class="gt_row gt_right">219</td>
<td headers="exponential_model" class="gt_row gt_right">208</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">10.8</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">12</td>
<td headers="scripts_reported" class="gt_row gt_right">205</td>
<td headers="exponential_model" class="gt_row gt_right">240</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">12.5</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">13</td>
<td headers="scripts_reported" class="gt_row gt_right">285</td>
<td headers="exponential_model" class="gt_row gt_right">276</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">14.4</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">14</td>
<td headers="scripts_reported" class="gt_row gt_right">371</td>
<td headers="exponential_model" class="gt_row gt_right">318</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">16.5</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">15</td>
<td headers="scripts_reported" class="gt_row gt_right">384</td>
<td headers="exponential_model" class="gt_row gt_right">366</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">19.0</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">16</td>
<td headers="scripts_reported" class="gt_row gt_right">401</td>
<td headers="exponential_model" class="gt_row gt_right">421</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">21.9</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">17</td>
<td headers="scripts_reported" class="gt_row gt_right">462</td>
<td headers="exponential_model" class="gt_row gt_right">485</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">25.2</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">18</td>
<td headers="scripts_reported" class="gt_row gt_right">NA</td>
<td headers="exponential_model" class="gt_row gt_right">558</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">29.0</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">19</td>
<td headers="scripts_reported" class="gt_row gt_right">NA</td>
<td headers="exponential_model" class="gt_row gt_right">642</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">33.4</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">20</td>
<td headers="scripts_reported" class="gt_row gt_right">NA</td>
<td headers="exponential_model" class="gt_row gt_right">739</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">38.4</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">21</td>
<td headers="scripts_reported" class="gt_row gt_right">NA</td>
<td headers="exponential_model" class="gt_row gt_right">851</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">44.3</td></tr>
  </tbody>
  &#10;</table>
</div>

![](Tonmya_prescriptions_files/figure-gfm/scripts%20exponential%202-1.png)<!-- -->
\## scripts Projection - at weekly rate - *linear model*

    ## 
    ## Call:
    ## lm(formula = scripts ~ wk, data = df_scripts)
    ## 
    ## Residuals:
    ##     Min      1Q  Median      3Q     Max 
    ## -71.221 -28.760   3.853  26.088  49.627 
    ## 
    ## Coefficients:
    ##             Estimate Std. Error t value Pr(>|t|)    
    ## (Intercept)  -50.544     18.932   -2.67   0.0175 *  
    ## wk            27.230      1.848   14.74 2.49e-10 ***
    ## ---
    ## Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1
    ## 
    ## Residual standard error: 37.32 on 15 degrees of freedom
    ## Multiple R-squared:  0.9354, Adjusted R-squared:  0.9311 
    ## F-statistic: 217.2 on 1 and 15 DF,  p-value: 2.488e-10

<div id="jdconedhml" style="padding-left:0px;padding-right:0px;padding-top:10px;padding-bottom:10px;overflow-x:auto;overflow-y:auto;width:auto;height:auto;">
<style>#jdconedhml table {
  font-family: system-ui, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol', 'Noto Color Emoji';
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
&#10;#jdconedhml thead, #jdconedhml tbody, #jdconedhml tfoot, #jdconedhml tr, #jdconedhml td, #jdconedhml th {
  border-style: none;
}
&#10;#jdconedhml p {
  margin: 0;
  padding: 0;
}
&#10;#jdconedhml .gt_table {
  display: table;
  border-collapse: collapse;
  line-height: normal;
  margin-left: auto;
  margin-right: auto;
  color: #333333;
  font-size: 16px;
  font-weight: normal;
  font-style: normal;
  background-color: #FFFFFF;
  width: auto;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #A8A8A8;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #A8A8A8;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
}
&#10;#jdconedhml .gt_caption {
  padding-top: 4px;
  padding-bottom: 4px;
}
&#10;#jdconedhml .gt_title {
  color: #333333;
  font-size: 125%;
  font-weight: initial;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-color: #FFFFFF;
  border-bottom-width: 0;
}
&#10;#jdconedhml .gt_subtitle {
  color: #333333;
  font-size: 85%;
  font-weight: initial;
  padding-top: 3px;
  padding-bottom: 5px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-color: #FFFFFF;
  border-top-width: 0;
}
&#10;#jdconedhml .gt_heading {
  background-color: #FFFFFF;
  text-align: center;
  border-bottom-color: #FFFFFF;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}
&#10;#jdconedhml .gt_bottom_border {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}
&#10;#jdconedhml .gt_col_headings {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}
&#10;#jdconedhml .gt_col_heading {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 6px;
  padding-left: 5px;
  padding-right: 5px;
  overflow-x: hidden;
}
&#10;#jdconedhml .gt_column_spanner_outer {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  padding-top: 0;
  padding-bottom: 0;
  padding-left: 4px;
  padding-right: 4px;
}
&#10;#jdconedhml .gt_column_spanner_outer:first-child {
  padding-left: 0;
}
&#10;#jdconedhml .gt_column_spanner_outer:last-child {
  padding-right: 0;
}
&#10;#jdconedhml .gt_column_spanner {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 5px;
  overflow-x: hidden;
  display: inline-block;
  width: 100%;
}
&#10;#jdconedhml .gt_spanner_row {
  border-bottom-style: hidden;
}
&#10;#jdconedhml .gt_group_heading {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  text-align: left;
}
&#10;#jdconedhml .gt_empty_group_heading {
  padding: 0.5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: middle;
}
&#10;#jdconedhml .gt_from_md > :first-child {
  margin-top: 0;
}
&#10;#jdconedhml .gt_from_md > :last-child {
  margin-bottom: 0;
}
&#10;#jdconedhml .gt_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  margin: 10px;
  border-top-style: solid;
  border-top-width: 1px;
  border-top-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  overflow-x: hidden;
}
&#10;#jdconedhml .gt_stub {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 5px;
  padding-right: 5px;
}
&#10;#jdconedhml .gt_stub_row_group {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 5px;
  padding-right: 5px;
  vertical-align: top;
}
&#10;#jdconedhml .gt_row_group_first td {
  border-top-width: 2px;
}
&#10;#jdconedhml .gt_row_group_first th {
  border-top-width: 2px;
}
&#10;#jdconedhml .gt_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}
&#10;#jdconedhml .gt_first_summary_row {
  border-top-style: solid;
  border-top-color: #D3D3D3;
}
&#10;#jdconedhml .gt_first_summary_row.thick {
  border-top-width: 2px;
}
&#10;#jdconedhml .gt_last_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}
&#10;#jdconedhml .gt_grand_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}
&#10;#jdconedhml .gt_first_grand_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-style: double;
  border-top-width: 6px;
  border-top-color: #D3D3D3;
}
&#10;#jdconedhml .gt_last_grand_summary_row_top {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-style: double;
  border-bottom-width: 6px;
  border-bottom-color: #D3D3D3;
}
&#10;#jdconedhml .gt_striped {
  background-color: rgba(128, 128, 128, 0.05);
}
&#10;#jdconedhml .gt_table_body {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}
&#10;#jdconedhml .gt_footnotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}
&#10;#jdconedhml .gt_footnote {
  margin: 0px;
  font-size: 90%;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
}
&#10;#jdconedhml .gt_sourcenotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}
&#10;#jdconedhml .gt_sourcenote {
  font-size: 90%;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
}
&#10;#jdconedhml .gt_left {
  text-align: left;
}
&#10;#jdconedhml .gt_center {
  text-align: center;
}
&#10;#jdconedhml .gt_right {
  text-align: right;
  font-variant-numeric: tabular-nums;
}
&#10;#jdconedhml .gt_font_normal {
  font-weight: normal;
}
&#10;#jdconedhml .gt_font_bold {
  font-weight: bold;
}
&#10;#jdconedhml .gt_font_italic {
  font-style: italic;
}
&#10;#jdconedhml .gt_super {
  font-size: 65%;
}
&#10;#jdconedhml .gt_footnote_marks {
  font-size: 75%;
  vertical-align: 0.4em;
  position: initial;
}
&#10;#jdconedhml .gt_asterisk {
  font-size: 100%;
  vertical-align: 0;
}
&#10;#jdconedhml .gt_indent_1 {
  text-indent: 5px;
}
&#10;#jdconedhml .gt_indent_2 {
  text-indent: 10px;
}
&#10;#jdconedhml .gt_indent_3 {
  text-indent: 15px;
}
&#10;#jdconedhml .gt_indent_4 {
  text-indent: 20px;
}
&#10;#jdconedhml .gt_indent_5 {
  text-indent: 25px;
}
&#10;#jdconedhml .katex-display {
  display: inline-flex !important;
  margin-bottom: 0.75em !important;
}
&#10;#jdconedhml div.Reactable > div.rt-table > div.rt-thead > div.rt-tr.rt-tr-group-header > div.rt-th-group:after {
  height: 0px !important;
}
</style>
<table class="gt_table" data-quarto-disable-processing="false" data-quarto-bootstrap="false">
  <thead>
    <tr class="gt_heading">
      <td colspan="4" class="gt_heading gt_title gt_font_normal gt_bottom_border" style><span class='gt_from_md'>Linear Model</span></td>
    </tr>
    &#10;    <tr class="gt_col_headings">
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="wk">wk</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="scripts_reported">scripts_reported</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="linear_model">linear_model</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="yearly_rate_predicted_M">yearly_rate_predicted_M</th>
    </tr>
  </thead>
  <tbody class="gt_table_body">
    <tr><td headers="wk" class="gt_row gt_right">1</td>
<td headers="scripts_reported" class="gt_row gt_right">2</td>
<td headers="linear_model" class="gt_row gt_right">27.2</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">1.4</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">2</td>
<td headers="scripts_reported" class="gt_row gt_right">12</td>
<td headers="linear_model" class="gt_row gt_right">54.5</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">2.8</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">3</td>
<td headers="scripts_reported" class="gt_row gt_right">35</td>
<td headers="linear_model" class="gt_row gt_right">81.7</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">4.2</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">4</td>
<td headers="scripts_reported" class="gt_row gt_right">60</td>
<td headers="linear_model" class="gt_row gt_right">108.9</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">5.7</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">5</td>
<td headers="scripts_reported" class="gt_row gt_right">126</td>
<td headers="linear_model" class="gt_row gt_right">136.2</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">7.1</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">6</td>
<td headers="scripts_reported" class="gt_row gt_right">154</td>
<td headers="linear_model" class="gt_row gt_right">163.4</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">8.5</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">7</td>
<td headers="scripts_reported" class="gt_row gt_right">127</td>
<td headers="linear_model" class="gt_row gt_right">190.6</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">9.9</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">8</td>
<td headers="scripts_reported" class="gt_row gt_right">108</td>
<td headers="linear_model" class="gt_row gt_right">217.8</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">11.3</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">9</td>
<td headers="scripts_reported" class="gt_row gt_right">163</td>
<td headers="linear_model" class="gt_row gt_right">245.1</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">12.7</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">10</td>
<td headers="scripts_reported" class="gt_row gt_right">193</td>
<td headers="linear_model" class="gt_row gt_right">272.3</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">14.2</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">11</td>
<td headers="scripts_reported" class="gt_row gt_right">219</td>
<td headers="linear_model" class="gt_row gt_right">299.5</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">15.6</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">12</td>
<td headers="scripts_reported" class="gt_row gt_right">205</td>
<td headers="linear_model" class="gt_row gt_right">326.8</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">17.0</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">13</td>
<td headers="scripts_reported" class="gt_row gt_right">285</td>
<td headers="linear_model" class="gt_row gt_right">354.0</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">18.4</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">14</td>
<td headers="scripts_reported" class="gt_row gt_right">371</td>
<td headers="linear_model" class="gt_row gt_right">381.2</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">19.8</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">15</td>
<td headers="scripts_reported" class="gt_row gt_right">384</td>
<td headers="linear_model" class="gt_row gt_right">408.5</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">21.2</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">16</td>
<td headers="scripts_reported" class="gt_row gt_right">401</td>
<td headers="linear_model" class="gt_row gt_right">435.7</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">22.7</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">17</td>
<td headers="scripts_reported" class="gt_row gt_right">462</td>
<td headers="linear_model" class="gt_row gt_right">462.9</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">24.1</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">18</td>
<td headers="scripts_reported" class="gt_row gt_right">NA</td>
<td headers="linear_model" class="gt_row gt_right">490.1</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">25.5</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">19</td>
<td headers="scripts_reported" class="gt_row gt_right">NA</td>
<td headers="linear_model" class="gt_row gt_right">517.4</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">26.9</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">20</td>
<td headers="scripts_reported" class="gt_row gt_right">NA</td>
<td headers="linear_model" class="gt_row gt_right">544.6</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">28.3</td></tr>
    <tr><td headers="wk" class="gt_row gt_right">21</td>
<td headers="scripts_reported" class="gt_row gt_right">NA</td>
<td headers="linear_model" class="gt_row gt_right">571.8</td>
<td headers="yearly_rate_predicted_M" class="gt_row gt_right">29.7</td></tr>
  </tbody>
  &#10;</table>
</div>

![](Tonmya_prescriptions_files/figure-gfm/scripts%20linear-1.png)<!-- -->
