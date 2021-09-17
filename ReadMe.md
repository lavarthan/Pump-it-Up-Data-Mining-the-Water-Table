# Pump it Up: Data Mining the Water Table


## data exploration
  * generate statstics of the dataset
  * generate the percentage of the missing value in each columns
  * generate the uniques values of each columns and the total count for each values
  * checked every columns and analyse the similarity between the columns
  * imbalanced target values
  * some are the conclusion from the exploration
      * Mostly of the wells, funded by government are non-functional.
      * Most of water points,  central government and district council installed are non-functional
      * there is high percentage of well are non functional even it has water
      * wells near good basins have clean water

## preprocessing
  * removed null values based on the column type and the data
  * check the similarity between columns and droped it
  * removed columns which has higher number of null values
  * there were lot of misspellings, tried most of it into same value
  * categorical encoding, scaling done

## feature engineering
  * construction year field does not make sense in the dataset so i converted into a decade

## modeling
  * tried different type of classifiers for accuracy checking (LGBM, XGBoost, XGBoost with smote)
  * XGBoost with smote was very fast and the acuuracy was high than other models 
     * Training set accuracy 0.9702793815631418
     * Test set accuracy 0.8621616036371151

## feauture importance
  * finally done feauture imporatnce to make the model better. Training accuracy was slightly lower than before and testing accuracy is slightly high
     *  Training set accuracy 0.9687552472843285
     *  Test set accuracy 0.8632833230006199

![Feauture imporatnce](https://github.com/lavarthan/Pump-it-Up-Data-Mining-the-Water-Table/blob/master/feauture_imporatancepng.png)


