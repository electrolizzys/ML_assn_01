ეს პროექტი არის  House Prices - Advanced Regression Techniques.
მისი მიზანია საცხოვრებელი სახლების ფასების წინასწარმეტყველება მახასიათებლების მიხედვით. შეფასება ხდება RMSLE-ით.

პრობლემის გადასაჭრელად გამოყენებული იქნა Preprocessing, Feature Engineering, Feature Selection, სხვადასხვა რეგრესიის მოდელის ტესტირება და Grid Search. 

1.კატეგორიული ცვლადების რიცხვითში გადაყვანა One-Hot Encoding-ით, იმ შემთხვევაში თუ სვეტში 3-ზე ნაკლები ან ტოლი რაოდენობის განსხვავებული მახასიათებლები გვხვდება. 
სხვა შემთხვევაში WOE ენქოუდინგი.
2.ნულოვანი პარამეტრების დაჰენდლვა კატეგორიული და ნუმერიქალების გათვალისწინებით. 80%-ზე მეტი ნულოვნის შემთხვევაში ამოვარდა სვეტები.
3.მაღალი კორელაციის მქონე სვეტები ამოვარდა.

Feature Selection
RFE და მაღალი კორელაციის გათვალისწინებით

linearRegression(Lasso) 
RandomForestRegressor

model-experiment.ipynb — მოიცავს მონაცემების დამუშავებას, Feature Engineering-ს, სხვადასხვა მოდელის გადამზადებას (Random Forest, Linear Regression) და მათ შეფასებას.
model-inference.ipynb — ფოკუსირებულია საბოლოოდ შერჩეული მოდელის გამოყენებით პროგნოზის შესრულებაზე.

Random Forest მოდელს overfitting-ისკენ,ამის თავიდან ასაცილებლად მოხდა კროსვალიდაციის შედეგების შეფასება, Feature Selection - სვეტების მოცილებით.
საუკეთესო მოდელის შედეგები:
მოდელი არჩეულია მიღწეული მეტრიკების საფუძველზე, რომლებიც აჩვენებენ მის სიზუსტეს და სტაბილურობას სხვადასხვა მონაცემზე.
RMSLE  0.14523618002742475 



https://dagshub.com/electrolizzys/ML_assn_01.mlflow/#/experiments/0?searchFilter=&orderByKey=attributes.start_time&orderByAsc=false&startTime=ALL&lifecycleFilter=Active&modelVersionFilter=All+Runs&datasetsFilter=W10%3D
# Readme
