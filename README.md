# frtproject
This is my repository that contains my project for my Future Ready Talent Internship. 

## Project Title:
Custom Design - Custom Apparels for You - With AI Chatbot for queries

## Problem Statement
This Project "Custom Design" basically showcases that small companies instead of hiring a huge amount of employees to solve Customer questions and queries can integrate Chatbot to their websites powered by AI to solve common queries of customers in chat format, reducing the man-power.

## Project Description:
The core idea of the project is to enhance customer support and engagement for a small company specializing in custom apparel creation (e.g., t-shirts, coffee mugs) through the implementation of a Custom AI Bot on their website.

The problem being addressed is the common issue of customer queries and concerns, which can be time-consuming for both customers and the company to address manually. Traditional customer support channels may lead to delays, especially during peak times or outside regular business hours. The project aims to streamline and expedite customer interactions by providing an AI-driven solution that can handle common queries efficiently.

The project solves this problem by integrating a Custom AI Bot that understands and responds to frequently asked questions. With natural language processing capabilities, the AI Bot can comprehend and respond like a human. By automating, customer support agents are not only freed up to provide prompt and accurate support.

Project functionality and purpose are intricately mapped to identified problem statements. It aims to improve customer satisfaction by providing real-time assistance and resolving queries. The solution is explained clearly through the integration of the AI Bot, which is prominently featured on the website and designed to guide users through the query resolution process.

In summary, the project's core idea revolves around leveraging AI technology to address the common problem of time-consuming customer queries in the custom apparel industry. The purpose and functionality of the Custom AI Bot align closely with the identified problem, providing an efficient and effective solution to enhance customer support and overall user experience on the company's website.

## Project Building:
The first thing I did was to create a resource group on the Azure Portal for the Project. In that resource group, I created an Azure Language Resource and went to Azure Language Studio. There I created a Custom QuestionAnswering project after choosing my Subscription and other details.
![7](https://github.com/manglanivivek/frtproject/assets/120302143/d4f06b17-d649-41ae-956d-0020f3b01f3c)
Then I opened the project and added answer pairs to the Knowledge Base manually and some questions from the chitchat source.
![9](https://github.com/manglanivivek/frtproject/assets/120302143/105d0b03-3743-473d-8296-76ae0325d910)
Questions of the answer pairs that I gave the knowledge base were:
Can I expedite the shipping of my custom order?
How long does it take to receive my custom order?
What types of custom products do you offer?
Where is your company located?
How can I contact your customer service?
Are there any discounts for bulk orders?
How are your prices determined for custom products?
What is your return policy?

After that I deployed my Knowledge Base.
![10](https://github.com/manglanivivek/frtproject/assets/120302143/cdd452c0-dcad-4208-afbe-f84eeb7115b3)
Now it was time to create a bot. I chose the create bot option and created one using the resource key of my Language Resource. After the completion of deployment of bot, my resouce group had the resources as shown below.
![11](https://github.com/manglanivivek/frtproject/assets/120302143/e68fc747-05e8-4469-8d86-9002a5d2cda9)
Now, to integrate my bot with my website, I went to the channels section of my bot's resource. There I got the embed code of my bot and I added it to my code.
![12](https://github.com/manglanivivek/frtproject/assets/120302143/aa22bdbe-c147-4ced-94b4-2ff29c3b9ce8)
![17](https://github.com/manglanivivek/frtproject/assets/120302143/56769576-10e3-4237-9434-fcb1d830ca3b)

Now, I had to deploy my static website. To deploy my static website, I used the Static Web Apps service provided in the Azure Storage Account. The reason I deployed it using the Storage Account is because Storage Account provides advantages for statics websites like Cost Efficiency, Scalability and many more.
To achieve this, I first created a storage account resource in the same resource group.
![14](https://github.com/manglanivivek/frtproject/assets/120302143/ec985b9e-905a-496d-ae45-520b6e9965bc)
Then I enabled the static website option in the storage account.
![15](https://github.com/manglanivivek/frtproject/assets/120302143/873250bb-6a52-416c-9b57-73935e6a70e5)
Now, a "$web" container was created in the storage account. This is were we have to upload our website files. So here I uploaded all the files of my website.
![16](https://github.com/manglanivivek/frtproject/assets/120302143/34e4de84-d6bb-4515-8817-63059df02826)
And my Static Website with an AI QnA Bot using Storage Account and Azure AI has been deployed. Below are some photos from my website.
![1](https://github.com/manglanivivek/frtproject/assets/120302143/faea818d-5245-480e-861c-5565c24d0aac)
![2](https://github.com/manglanivivek/frtproject/assets/120302143/7c0de2ce-a366-46fc-8f38-da90b99c8aa2)
![3](https://github.com/manglanivivek/frtproject/assets/120302143/881e630c-4f09-4e04-9fc1-ba0b6890083c)
![4](https://github.com/manglanivivek/frtproject/assets/120302143/d78a7ca7-b246-421a-a367-b77faa97ac7b)
![6](https://github.com/manglanivivek/frtproject/assets/120302143/b57b2c64-aa8f-4c44-b04d-361815108add)




