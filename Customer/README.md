<div>
  <h1>User Research on Style preference</h1>
  <img src = "images/recommendation.png" width = 90%>
  <h2><b>Background</b></h2>
  <p>This is a user research project in a fashion e-commerce startup at Taiwan in 2021.<br>
    Back then, our important operational KPI was Average Order Value(AOV).<br>
    Since the launch of the service, this number had been around 2000 TWD. <br>
  </p>
  <h2><b>Objective</b></h2>
  <p>My Mission was to find a product improvement opportunity to enhance this KPI.</p>

  <h2>Data Source</h2>
  <ul>
    <li>Order Data with cusotmer ID (e.g. datetime, product_ID, customer_ID, return_status, etc)</li>
    <li>Product Data(e.g. product_ID, product_name, product_page_url, brand_ID, etc)</li>
    <li>User action data from Google Analytics(e.g. pageview, screen scrool, click etc)</li>
    <p><font color="red">*all data was from 2020/03~2021/8</font></p>
  </ul>

  <h2><b>Approach</b></h2>
  <p>I ran both quantitative and qualitative analysis for this project.</p>
  <h3>1. Qualitative Analysis</h3>

  <p>In the user interviews with our loyal customers, we realized our recommendation lacked diversity in fashion styles. From here, we created hypothesis that recommending more diverse products would contribute user satisfaction.</p>
  <h3>2. Quantitative Analysis (the main point of this notebook!)</h3>
  <p>
  Next, I tried to validate this hypothesis by checking whether the users who interacts with a variety of styles buy more products per order than the users who like a limited number of styles.<br>
  For this purpose, I first create a new dataset describing style of each brand, by working with our stylist team.<br> 
  The new dataset is style-brand mapping table, which contains brand_ID, style_ID, style_name. As a sidenote, we defined 13 different styles in fashion.<br>
  Then, we calculated the distribution of style preference from product data, order data, and pageview data for each person. <br>
  For example, one could have a preference like Sport 50%, Natural 30%, Street 20%, and 0% for the rest 10 styles.<br><br></p>
  <img src = "images/example_style_preference.png" width = 90%>
  <p><br><br>Then I clustered them into 5 groups by the distribution of style preference.</p>
  <br>
    <img src = "images/graph_5groups.png" width = 60%>
    <img src = "images/performance_5groups.png" width = 100%>



<h2><b>Result</b></h2>
<p>
  It turned out the more various styles a user prefers, the more they spend with more frequency.
  <br><b>The group with the most diverse preference(RAINBOW) spend 56% more than the group with the least diverse preference(MINIMALIST).</b><br></p><br>
      <img src = "images/result.png" width = 50%>
  <p><br>Thus our hypothesis was validated. <br>
  After that, we worked on this opportunity and improved our recommendation on another project, it increased the KPI by <b>15%</b>.</p>
</div>
