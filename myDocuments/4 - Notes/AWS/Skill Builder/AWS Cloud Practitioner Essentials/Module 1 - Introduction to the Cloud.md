---
Index: "[[3 - Indexes/AWS/AWS Cloud Practitioner Essentials|AWS Cloud Practitioner Essentials]]"
tags:
  - cloud
  - certification
  - aws
---
# Introduction
**Rudy:** Hey everyone! Welcome to the course. We hope you're ready to dive in and learn the fundamentals of the AWS cloud.

**Alan:** We have a lot of material to cover. And we're going to start with defining; what is the cloud?

**Morgan:** But, before we do that, let's start with some introductions. Hi, I'm Morgan Willis, a Principal Cloud Technologist with AWS Training and Certification. I started in the IT world about 15 years ago. And along the way, I decided that I was missing something.

I missed the helping and teaching aspect that I had in my first job in IT support. So, I went into teaching at a software development bootcamp. And then I eventually landed here at Amazon Web Services, or AWS, where, as a Cloud Technologist, I get to support others in their cloud learning journey every day.

**Rudy:** Howzit learners! My name is Rudy Chetty and I'm a Chief Techfluencer and a Principle Solutions Architect for AWS Partners. I'm originally from sunny Cape Town, South Africa…the home of bunny chow, biltong and boerewors. I've been in the technology space for over two decades helping customers worldwide realize their application and cloud dreams. Education is my passion. Therefore, I cannot wait for you to dive into this course and learn all about the wonders of the cloud and AWS.

**Alan:** And I'm Alan Meridian. I'm an instructor in AWS Training and Certification.

Over the last eight plus years with AWS, I've delivered hundreds of trainings introducing learners like you to AWS concepts, services, and solutions-sometimes involving ukuleles. I'm glad you're here. We're going to learn a lot together.

**Rudy:** Look, cloud computing can be complex. But don’t worry. This is why we’re here! Our curriculum provides analogies, examples, and use cases that will help you better understand these concepts. We’ll cover all the essential information you need to be comfortable discussing AWS. Additionally, we'll throw in some AWS service demos to show you how things work in action. This layered approach to learning will really reinforce concepts. Oh, and we promise to keep it simple.

**Morgan:** AWS offers a massive range of services for every business. AWS is the world's most comprehensive and broadly adopted cloud, and millions of customers use AWS to be more agile, lower costs, and innovate faster. Whether you're looking for compute power, generative AI, databases, storage, content delivery, or specialized services for some other functionality, AWS has the services you need to help you build sophisticated applications for your business.

**Alan:** That is massive range of services, and I wish we had time to cover them all. But, we did promise to keep it simple. So, let's start this conversation with a fundamental concept of computing: the client-server model.

**Rudy:** And to get things percolating in your brain, we are going to brew up a coffee shop analogy. This coffee shop is going to act as a real-world metaphor to show you the different parts of the cloud computing model. And, the analogy will help you understand how AWS can change the way your IT operates.

First, let's think about the coffee shop and how it can represent the client-server model.

**Alan:** Let's have Morgan be the server, the barista. And I'll be the client, or the customer. I'm gonna make a request. In this case, it's for coffee. In the computing world, the request could be for anything. It could be rain pattern analysis in South Africa, or it could be the latest x-rays of your knee, or videos of kittens. Whatever the business needs is where the request starts. Basically, a customer makes a request, and with permissions, the server responds to that request. All I want is a caffeinated beverage. Morgan represents the server part of the client-server model. In AWS, she would be a virtual server. So, from a cloud computing architectural point of view, the coffee shop transaction is pretty straightforward. I, the user, made a request to Morgan, the server. Morgan validated that the request was legitimate. In this case, did I give her money? Is the item that I ordered something that they can make? Then she returned a response, which in this example, is a triple mocha with extra caramel shots.

**Morgan:** Now, in the real world, applications are usually more complicated than just a single transaction with a single server. In a business solution that is more mature, it can get beautifully complex. But again, we're going to start with the basics. As the curriculum progresses, these basic concepts will continue to build on each other. And hopefully, by the end, those beautifully complex concepts will make a lot more sense. You've already tackled your first cloud computing concept. So now, let's continue with a key concept of AWS, and that is, you only pay for what you use.

**Rudy:** Think about this principle as it applies to staffing a coffee shop. Employees are only paid for the hours they work in the actual shop. So, if say Morgan and I are off the clock, well, then we don't get paid because we didn’t work any hours. Moreover, the store owner decides how many baristas they need for any given day of the week. Busy days require more employees and slower days require fewer. Let’s take an example. Say the coffee shop is releasing a brand-new drink called Rudy’s Rhubarb Refresher. Trademark. The shop anticipates increased demand due to the beverage being very tasty, so they staff the shop with 10 baristas all day long. Although this works with a sudden surge of customers, it isn’t great for slower periods during the day. Some baristas could be idle, and it would be hard to justify paying them to just be there in case they are needed. The monetary cost just doesn’t make good financial sense.

**Alan:** And yet, this is exactly what happens in an on-premises data center where you can't just snap your fingers and triple your capacity. At AWS, you don't pre-pay for anything. And you don't have to worry about capacity constraints.

**Rudy:** When you need more resources, you just provision them right then and there. How cool is that? Then, when you don't need those resources anymore, you can deprovision just as quickly. You just set up the right configuration and it’s done automatically. And the best part is that when you deprovision the resources, you stop paying for them immediately. Just like you only pay your employees for the hours they’re working, you only pay for the AWS resources that you consume.

**Morgan:** Right. So, paying only for what you use is the first AWS specific concept we covered—and it’s just one of the many benefits when it comes to running your business on AWS. And that's really why we're here: so you can understand how AWS is built to help you run your business better.

**Alan:** Exactly. You’ve already learned some foundational concepts about the cloud…and that’s just the start!

**Rudy:** Yep, things are only going to get more interesting, folks, as we dive deeper! Thanks for joining us on this learning journey, future AWS Cloud Practitioner. See you soon.

---
# What is Cloud Computing
**In this lesson, you will learn how to do the following:**
- Define cloud computing
- Describe and differentiate between cloud deployment types.

In today's technological world, you are probably familiar with the concept of the cloud, but you might not know the technical details of how cloud computing works. In this lesson, you learn the basic definition of cloud computing, and you explore how Amazon Web Services (AWS) helped pave the way for a new technological frontier.

---

Before we dive into cloud computing, let's rewind the clock and set some context for how Amazon grew to include Amazon Web Services. In the early 2000s, Amazon.com was an ecommerce site that customers used to buy books and other consumer goods. As more people started to use the site, the Amazon IT team had to continually make upgrades to keep things running smoothly. More servers, more storage, more compute. You name it. They were deploying it!

The team eventually decided to develop various standardized tools, mechanisms, and ways to make things more efficient and scalable. These methods proved to be quite effective, and in 2003, employees thought, "Maybe this knowledge would be valuable to other companies facing similar challenges." Thus, Amazon started to envision a service that would allow businesses to rent computing power, storage, and other resources, on-demand. This business model could eliminate the need for upfront investment in hardware.

Just a year later, in November 2004, AWS launched its first public infrastructure service: Amazon Simple Queue Service. Two years later, AWS launched Amazon Simple Storage Service for data storage and Amazon Elastic Compute Cloud for scalable compute. Initially, AWS was used by smaller start-ups and developers. However, its scalability, cost-effectiveness, and ease of use quickly attracted larger enterprises.

Over the next few years, AWS rapidly expanded its offerings by adding databases, networking, analytics, and many other cloud-based services. Fast forward to the present. AWS powers a significant portion of the internet, serving millions of customers worldwide. From small start-ups and businesses, to large corporations, government agencies, and more. What started as an internal solution for Amazon's own IT needs has grown into a global cloud computing leader.

With that quick history lesson in mind, let's look at a working definition of cloud computing. Cloud computing is essentially the on-demand delivery of IT resources over the internet with pay-as-you-go pricing. Shall we break this down a bit? I think we shall. On demand means you use resources as needed. Let's say your business needs 2,000 TB of storage. Open an AWS account, throw some files into Amazon S3, and Bob’s your uncle. You're good to go. If you don't need to store those files anymore? Delete them, and stop paying immediately.

The idea of the delivery of these on-demand IT resources, as you learned, is the concept that got AWS started in the first place. Let's say you have an application that you have to run, content you need stored, or data you need analyzed. Basically, you have stuff that uses IT resources that have to live and operate somewhere. All of that data is stored in a data center, which is essentially a building or set of buildings devoted to housing servers that contain all this data. Data centers are designed with redundant power, cooling, and security measures to ensure secure and continuous operation. Historically, businesses would run applications in their own data centers or co-locate with other customers in a shared facility. There was no alternative. Once AWS became available, companies could now run their applications in other data centers they didn't actually own. No more infrastructure to manage. No more repetitive tasks and time-consuming ones--goodbye. By using AWS, teams could now focus on innovation.

Oh, and the over-the-internet part means you can access those resources remotely. You can be in your house, place of business, or visiting family around the world. Hi Mom! In fact, all you need is an internet connection. Log into your AWS Account and manage your infrastructure right from your web-browser.

And with pay-as-you-go pricing, if you don’t need a particular part of your infrastructure, just deprovision it. Simple as that. No contracts. No need to call a sales rep.

To reiterate: cloud computing is the on-demand delivery of IT resources over the internet with pay-as-you-go pricing. So, as you tackle the rest of this content, keep this definition in mind. Happy learning!

## Cloud deployment types

You can deploy cloud resources in multiple ways: cloud, on-premises, and hybrid. Each type offers unique benefits and considerations, and exploring these options can help you make informed decisions about your cloud strategy. To learn more about cloud deployment types, choose each of the following flashcards.

### Cloud-bases deployment
In a cloud-based deployment model, you have the flexibility to migrate your existing resources to the cloud, design and build new applications within the cloud environment, or use a combination of both.

For instance, a company might migrate data resources to the cloud, then develop an application comprised of virtual servers, databases, and networking components entirely hosted in the cloud.

### On-premises deployment
Deploying resources on premises using virtualization and resource management tools does not provide many of the benefits of cloud computing. However, it is sometimes sought for its ability to provide dedicated resources and low latency.

In most cases this deployment model is the same as legacy IT infrastructure while using application management and virtualization technologies to try increasing resource utilization.

### Hybrid deployment
In a hybrid deployment, cloud-based resources and on-premises infrastructure work together. This approach is ideal for situations where legacy applications must remain on premises due to maintenance preferences or regulatory requirements.

For instance, a company might choose to retain certain regulated legacy applications on-premises while using cloud services for advanced data processing and analytics.

Multi-cloud deployments can also be considered hybrid deployments.

---

# Benefits of the AWS Cloud
**In this lesson, you will learn how to do the following:**
- Describe the six key benefits of cloud computing.
Now that you understand how the cloud operates at a fundamental level, you will explore some advantages of using the cloud for your business. In this lesson, you will learn about six key benefits of cloud computing.

Okay. You have a good working definition of cloud computing, and you've also touched on why it's beneficial from a business perspective. Now, you'll learn even more about the advantages of using a cloud computing model. We'll cover six primary benefits of the AWS Cloud.

Let's start by talking a bit more about that first concept we've mentioned: the ability to pay as you go. With the cloud, you can trade fixed expenses for variable expenses. Remember when we talked about how data is housed in a data center? When you’re building a traditional on-premises facility, you typically need to invest a large amount of money upfront. This includes investments in physical space, hardware, staff, and upkeep to make sure everything is running smoothly. For some businesses, this can be hundreds of thousands or even millions of dollars. Then, regardless of the data center's utilization rate, you have a fixed cost, and you have to set up your budget around that fixed cost.

Billing with AWS is fundamentally different. Your bill with AWS will be variable from month to month as you consume different amounts of resources. The great thing about this model is that if you’re just getting started, there's no need to come up with a big investment to build out your AWS environment. Instead, you can start small and get billed for only what you use. And, you can use built-in billing and budgeting tools to find ways to save money every month as your business grows. So, that's the first advantage.

The next advantage is that you benefit from massive economies of scale. AWS is building data centers all around the world. And in order to build all those data centers, AWS is buying a whole lot of hardware. Because AWS buys a good amount of hardware, we can purchase this hardware at a lower price. Then, we pass on those lower costs to the customer.

The next benefit? Stop guessing capacity. In a traditional data center, you purchase hardware based on projected usage. Let's say you estimate you'll have a user base of 10 million people over the next three years. That means you purchase enough hardware to support that growth over time. But what happens if, when that third year hits, you only have about 500,000 users? You're still stuck with the hardware you purchased to support 10 million users. Let’s flip the script. Imagine you underestimated your capacity. A growing customer base is great for your business, but the scramble to secure more hardware could be a real problem. You would need to rapidly procure more servers to handle that higher capacity. If you don’t adjust in time, your customers could have a degraded experience, or you might even lose them altogether.

This is the awesome part of AWS. You don't need to guess capacity. Scaling usually takes minutes, instead of the weeks or months it can take in an on-premises data center. You provision needed resources for the present. Then, you use scaling mechanisms to scale these resources up or down based on the day-to-day demand.

The next benefit is my personal favorite. Increase speed and agility. With AWS, you have more bandwidth to try new things. You can spin up test environments and run experiments, trying out new ways to solve a problem. And then, if that approach didn't work, you can just delete those resources and stop incurring cost. That way, you can spend less time provisioning and deprovisioning and more time innovating and optimizing.

Alright, next up. Stop spending money running and maintaining data centers. We've talked about the upfront cost of data centers, but there's more to it than that. Apart from the fixed cost of what it takes to build out a data center, AWS eases the cost of running and maintaining servers. This means instead of spending time and resources focusing on racking, stacking, and powering those servers, you’re spending more time focusing on customers.

And last but not least, we have go global in minutes. Let's say you're a company based in the US, and you want to expand your operations to India. Traditionally, you would need to run and operate data centers in India to effectively operate there. But with AWS, you don't need to do that on your own. You can instead deploy your applications to an AWS Region in India that is managed by AWS. The idea here is that the time it takes for you to expand into a secondary area of the world traditionally can be months or years. With AWS, it can just take minutes.

That's it. Those are the six main benefits of using the AWS Cloud. As you can tell, with AWS, your business can achieve cost savings, time savings, and the ability to tap into massive global infrastructure. As we continue to dive into the specifics of the infrastructure and services of AWS, it'll become more and more clear how your business can achieve these benefits.

---
## Key benefits of the AWS Cloud

The six key benefits of the AWS Cloud are as follows.

### Trade fixed expense for variable expense

By using the AWS Cloud, businesses can transition from fixed investments to variable costs. With variable costs, customer expenses are better aligned with actual usage, thus creating more financial flexibility.

### Benefit from massive economies of scale

Like buying a product in bulk can result in lower prices per unit, the vast global infrastructure of AWS can result in lower costs for customers. This means that AWS can be used by many organizations, from small startups to major corporations. Businesses big and small can access advanced technologies that were previously only accessible to large enterprises.

### Stop guessing capacity

Customers can dynamically scale AWS Cloud resources up or down based on real-time demand. This means businesses can achieve optimal performance without provisioning more or less infrastructure than they need.

### Increase speed and agility

With the cloud, businesses can rapidly deploy applications and services, accelerating time to market and facilitating quicker responses to changing business needs and market conditions.

### Stop spending money to run and maintain data centers

The AWS Cloud eliminates the need for businesses to invest in physical data centers. This means customers aren't required to spend time and money on utilities and ongoing maintenance. With AWS taking care of the physical infrastructure of the cloud, customer resources can be reallocated to more strategic initiatives.

### Go global in minutes

Businesses don't need to set up their own infrastructure to expand internationally. AWS provides a robust global infrastructure that customers can use to deploy applications and services across multiple areas in minutes.

---

# Introduction to AWS Global Infrastructure
**In this lesson, you will learn how to do the following:**
- Define AWS Regions and Availability Zones.
- Explain the benefits of high availability and fault tolerance.
    
In this lesson, you learn about the basics of the AWS Global Infrastructure. You learn about the unique physical setup of AWS resources, and you explore some benefits of AWS infrastructure, such as high availability and fault tolerance. You will learn about more advanced components of AWS infrastructure in a later lesson of this training. For now, it's helpful to have a fundamental understanding of basic AWS infrastructure elements, such as data centers, Availability Zones, and AWS Regions.

---

Let's talk about the AWS Global Infrastructure. You've already learned that AWS builds and maintains data centers around the world that you can use to go global in minutes, but there's a huge advantage to global reach that we haven't covered yet—and that's high availability.

To learn a little bit more about high availability, let's head back to our coffee shop. Say you've hired a new employee, and they're learning how to make a latte. They're doing awesome. They've got the right milk-to-espresso ratio, and they are even making some cool designs with their latte pour—until they miss the cup and they pour the latte all over the register. That is not good. The register is now fried, and it seems like it shorted the electricity everywhere in the shop. Yikes! That means we can't ring up the orders or make drinks for our customers. We're gonna have to close up shop until this is sorted out.

So, what does that mean for the business? Does this mean that the entire business isn't making any money until this is fixed? Well, luckily for us, we're prepared. The good news for our business—and for our customers—is that this isn't our coffee shop's only location. The shop is actually a chain, and we have locations all around the city. Customers can still get their coffee by visiting one of our shops just a few blocks away, and the business can continue even if one location is having a bad time.

So, whether an employee had a slight latte mishap, or a shop next door accidentally cut our internet line, or some other disaster keeps the shop from its day-to-day operations...no matter the reason, we know that our product will be highly available for our customers. They still get their coffee, and the business is still generating income. All is well.

AWS has a similar set up with our global infrastructure. It's risky to have one giant data center where all of the resources are housed. If something were to happen to that data center, like a power outage or a natural disaster, everyone's applications would go down all at once. You need high availability and fault tolerance. Let’s clarify those terms. High availability is all about making sure your applications stay accessible with minimal downtime. Even if one component fails, another is ready to pick up the slack so your service keeps running.

Fault tolerance takes it a step further by designing a system to continue to operate even if multiple components fail. It’s basically building resilience into every layer so that no one single failure brings down the whole system. Designing for high availability and fault tolerance is part of the reason why AWS operates in Regions, which are located in different areas around the world. These Regions are built to be as close to AWS customers as possible. This includes locations like Paris, Tokyo, Sao Paulo, Dublin, or Ohio.

Within each Region, we have what we call Availability Zones, or AZs. There are three or more AZs within a Region, for redundancy. We don't build AZs right next to each other, because if something like a natural disaster were to occur, you could lose connectivity to everything in that AZ. And continuing with the theme of redundancy, within each AZ, there is one or more discrete data centers with redundant power, networking, and connectivity.

So, if a Region is where all the pieces and parts of your application live, some of you might be thinking that we never actually solved the problem that we presented earlier. If my business needs to be disaster proof, then it can't run in just one location. Well, you're absolutely correct. That's why it's common for businesses to operate across multiple Regions. That way, if one Region is experiencing outages for any reason, the operations can failover to another Region...but we'll cover that in more depth in a later lesson.

In the meantime, I'm gonna sit back here and relax, because I know that my business is highly available regardless of any disasters...or spilled lattes.

---
## AWS Regions and Availability Zones

AWS Global Infrastructure consists of physical locations around the world that contain groups of data centers. To learn more about the design of AWS Regions and Availability Zones, choose each of the following two numbered markers.

## AWS Regions

AWS Regions are physical locations around the world that contain groups of data centers. These groups of data centers are called Availability Zones. Each AWS Region consists of a minimum of three physically separate Availability Zones within a geographic area.

## Availability Zones

An Availability Zone consists of one or more data centers with redundant power, networking, and connectivity. Regions and Availability Zones are designed to provide low-latency, fault-tolerant access to services for users within a given area.

## Availability Zones

An Availability Zone consists of one or more data centers with redundant power, networking, and connectivity. Regions and Availability Zones are designed to provide low-latency, fault-tolerant access to services for users within a given area.

## Achieving high availability with AWS Global Infrastructure
AWS infrastructure is designed with high availability and fault tolerance in mind. Availability Zones (AZs) are configured as isolated resources, and they are each equipped with independent power, networking, and connectivity.

It's recommended to distribute your resources across multiple AZs. That way, if one AZ encounters an outage, your business applications will continue to operate without interruption. With this approach of redundancy and resource isolation, AWS customers can achieve the benefits of high availability and fault tolerance.