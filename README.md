### Link to the Article：

[Instagram System Design](https://medium.com/@nikhilgupta1/instagram-system-design-f62772649f90)

### Why it is interesting and useful

this is article is about how to build an APP with the structre of Instagram, which is really helpful for those who want to make the project related to social media. The article introduced the design idea and what should be prioritized during the SNS APP development for backend(database, data storage, etc.) and front-end(user functions) functions.

For instance, the article mentioned that: The design considerations for the system include selecting appropriate data stores for storing uploaded images and user data.

** Data Store for Uploaded Images: **

 - Requirement: Quick retrieval and rendering of uploaded images.
 - Reliability: Ensure no loss of user-uploaded images.
 - Scalability: Ability to handle a vast number of images.
 - Low Latency: Fast retrieval of photos.
 - Solution: Consider using object storage, such as AWS S3, due to its low read latency and efficient management of a large number of records.

** Data Store for User Data and Uploads Metadata: **

 - Requirement: Store metadata of user uploads and user data.
 - Availability: High availability for user data access.
 - Low Latency: Minimal delay for read operations.
 - Scalability: Handle a massive volume of records.
 - Reliability: Support sharding and replication.
 - Solution: Opt for a key-value NoSQL database like AWS DynamoDB due to its suitability for these requirements.