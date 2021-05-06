# Informal Response 

For this module, I continued to use Cambodia. The first step was to download all of the data from both sites. The GAMD database was not working the first few tries I tried to download the data, but after a couple days of checking every few hours the data finally downloaded sucessfully and completely. There were no other problems getting data from Worldpop, and I was able to get a population raster for both 2019 and 2020, but I ended up using the raster from 2019 in the end. From the data in class, here are some figures I was able to create. 

#### Map of Cambodia 
This includes layers the first two administrative levels inside Cambodia. Only the first administration has levels though for optimal readability. 

![Cambodia2](https://user-images.githubusercontent.com/78227378/117348914-cfc47780-ae78-11eb-87c6-9426c9fffc57.png)

#### Rasterstack 
![rasterstack](https://user-images.githubusercontent.com/78227378/117345564-b15c7d00-ae74-11eb-855f-8ad866e33a2d.png)

Code:
``` python
 pop19_fit %>% collect_metrics()
# A tibble: 2 x 4
  .metric .estimator  .estimate .config             
  <chr>   <chr>           <dbl> <fct>               
1 rmse    standard   20812.     Preprocessor1_Model1
2 rsq     standard       0.0667 Preprocessor1_Model1
```

### Linear Regression
![Lin Reg results](https://user-images.githubusercontent.com/78227378/117354296-2c2a9580-ae7f-11eb-87dc-95df14ebcf49.png)

Variable Importance Chart:

![Lin Reg importance](https://user-images.githubusercontent.com/78227378/117354432-4f554500-ae7f-11eb-9b15-f259afbc3310.png)
