# Read: Class 18 : AWS: API, Dynamo and Lambda

---

## Review, Research, and Discussion

- **What are serverless functions?**

A serverless function is a programmatic function written by a software developer for a single purpose. It's then hosted and maintained on infrastructure by cloud computing companies. These companies take care of code maintenance and execution so that developers can deploy new code faster and easier.

- **If you were to create a system that emulated Lambda functions, how would you do it?**

  > - Open the Functions page on the Lambda console.
  > - Choose Create function.
  > - Under Basic information, do the following:
  > - For Function name, enter my-function.
  > - For Runtime, confirm that Node.js 14.x is selected. Note that Lambda provides runtimes for .NET (PowerShell, C#), Go, Java, Node.js, Python, and Ruby.
  > - Choose Create function
  >   Lambda creates a Node.js function and an execution role that grants the function permission to upload logs. The Lambda function assumes the execution role when you invoke your function, and uses the execution role to create credentials for the AWS SDK and to read data from event sources.

- **Describe how a CDN works**

Content Delivery Network is a geographically distributed group of servers that work together to provide fast delivery of Internet content. A CDN allows for the fast transfer of data needed for loading Internet content including HTML pages, javascript files, stylesheets, images, and videos. Employing a CDN doesn’t only speed up the delivery of Internet content, it helps protect your website against certain forms of cyber attacks, It protects against these threats because CDNs allow for the handling of more traffic and withstanding hardware failure better than many origin servers.

---

### Document the following Vocabulary Terms

- **Serverless Functions** A serverless function is a programmatic function written by a software developer for a single purpose. It's then hosted and maintained on infrastructure by cloud computing companies. These companies take care of code maintenance and execution so that developers can deploy new code faster and easier

- **Cloud Storage** Cloud storage is a model of computer data storage in which the digital data is stored in logical pools, said to be on "the cloud". The physical storage spans multiple servers, and the physical environment is typically owned and managed by a hosting company.

- **CDN** Content Delivery Network geographically distributed group of servers that work together to provide fast delivery of Internet content. A CDN allows for the fast transfer of data needed for loading Internet content including HTML pages, javascript files, stylesheets, images, and videos.

---

## Preview

Which 3 things had you heard about previously and now have better clarity on?

--

Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

--

What are you most excited about trying to implement or see how it works?

--

---

**Amazon DynamoDB** is a key-value and document database that delivers single-digit millisecond performance at any scale. a hosted NoSQL database offered by Amazon Web Services (AWS). It offers:
reliable performance even as it scales;
a managed experience, so you won't be SSH-ing into servers to upgrade the crypto libraries
a small, simple API allowing for simple key-value access as well as more advanced query patterns.

**Amazon API Gateway**  
Amazon API Gateway is a managed service that allows developers to define the HTTP endpoints of a REST API or a WebSocket API and connect those endpoints with the corresponding backend business logic. It also handles authentication, access control, monitoring, and tracing of API requests.  
API Gateway handles all the tasks involved in accepting and processing up to hundreds of thousands of concurrent API calls, including traffic management, CORS support, authorization and access control, throttling, monitoring, and API version management
![](https://d1.awsstatic.com/serverless/New-API-GW-Diagram.c9fc9835d2a9aa00ef90d0ddc4c6402a2536de0d.png)
