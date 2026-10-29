# ai-ecommerce-recommendation-system
# ShopWise — AI E-Commerce Recommendation System

ShopWise is a demonstration web app that recommends sample products based on a visitor’s selected interest: Running, Fitness, or Outdoors. It displays product names, prices, and explanations for the recommendations.

## Live demo

[Open ShopWise](https://d3irjghc2j7szu.cloudfront.net)

## How it works

1. The visitor chooses an interest on the website.
2. Amazon API Gateway sends the request to an AWS Lambda function.
3. The Lambda function uses Amazon Bedrock (Nova 2 Lite) to generate recommendations from a sample product catalog.
4. The results are returned to the website and saved in Amazon DynamoDB.

## AWS services

- **Amazon S3** stores the website files.
- **Amazon CloudFront** delivers the website.
- **Amazon API Gateway** receives recommendation requests.
- **AWS Lambda** handles the backend logic.
- **Amazon Bedrock** generates the recommendation explanations.
- **Amazon DynamoDB** stores recommendation results.
- **Amazon CloudWatch** keeps function logs.

## Try it

Open the live demo and select **Running**, **Fitness**, or **Outdoors** to see recommendations for that interest.

## Note

This is a learning demo using a sample product catalog. Recommendations are for demonstration purposes.
