# Predictive-Modelling-Breast-Cancer-Dataset
## :dart: Goal
In today’s world, majority of the women are experiencing breast cancer as it has become a common diagnosis. After treatment, the recurrence of cancer can be frightening to them. A few studies conducted shows that breast cancer returns in women after 3-5 year of their treatment. The recurrence of the breast cancer can be maintained by either surgery, chemo radiation, or some form of medical treatment. 
<br><br>
The purpose of this project is to predict if a woman is likely to have a recurrence of a breast cancer even after their treatment. We would be creating a **classification model** to achieve the goal. The findings from predictive modelling could help oncologist diagnose cancer recurrence sooner *(especially in asymptomatic women)* and help understand what measure could be done to prevent the recurrence soon.  

####  :large_blue_diamond: Data MetaData <br>

Variable | Description | Datatype | Invalid Data | Missing Values
| :---: | :---: | :---: | :---: | :---:
Class  | Recurring or not recurring  | Nominal | No | No
Age | Age of patient at the time of diagnosis |Nominal | No | No
Menopause |Patient is premenopausal or post menopause| Nominal | No |No
Tumour -Size | Size of tumour in mm | Nominal | **Yes** | No
Inv-nodes | The number of lymph node that contains cancer | Nominal |**Yes** | No
Node-Caps | Has cancer penetrated to the capsule of lymph node | Nominal | No |**Yes**
Breast | Left or Right breast? | Nominal | No | No
Breast- Quadrant | Which quadrant of breast | Nominal | No |**Yes**
Irradiation | Exposed to radiation therapy. | Nominal | No | No
Degreee of Malignancy | Degree of malignant cancer | **Interval** | No | No


 #### :large_blue_diamond: Data Cleaning
 * Deleted the rows having missing values
* Transformed the values in ‘inv-node’ and ‘tumour size’ in the appropriate values using the formula “= Text (“value”, “format”) to convert date format to text.

 #### :large_blue_diamond: EDA and Predictive Modelling
 
The steps that were performed are as follows :
1. **StatExplore:** To explore the dataset and form some hypothesis. 
2. **Data Partition:**
    1. Training data - 70% 
    2. Validation dataset - 30%
3. **Replacement:** Replacing the values of class variable as following:
      1. Non-Recurrence : 0
      2.  Recurrence : 1
4. **Predictive Modelling**
    1. Decision Tree
    2. Logistic Regression
5. **Model Comparision**



