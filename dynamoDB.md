### JS commands for Dynamo DB

Call the SDK moduke and then use the following commands in the relevant functions:

General resource link here: https://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/DynamoDB.html

[Intro Video](https://www.youtube.com/watch?v=RLxWobyd2Tc)

---Core---

#### CRUD

[Update Item](https://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/DynamoDB.html#updateItem-property)

[Get Item](https://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/DynamoDB.html#getItem-property)

[Put Item](https://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/DynamoDB.html#putItem-property)


#### Methods

[Scan](https://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/DynamoDB.html#scan-property) 

[Query](https://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/DynamoDB.html#query-property)

#### Using DynamoDB locally

[Steps](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/DynamoDBLocal.html)

---Non-Core---

#### Disables Deal/Coupon

[Update Time To Live](https://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/DynamoDB.html#updateTimeToLive-property) <-- to look at implementing once we have basic functionality

---No-Go---

#### Tagging

[What is tagging?](https://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/DynamoDB.html#listTagsOfResource-property) <-- relates to monitoring for billing purposes so ignore

#### Secondary Indexes

This is global secondary index which costs, we need to use local secondary indexes:

[Global secondary index](https://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/DynamoDB.html#updateTable-property) < -- ignore not relevant . Best to create a "type" where we define it as Profile, Deal or Coupons with a primary key of the owner login credentials in all instances


