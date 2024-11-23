### Project Title
Phishing Email Classification
**Author**
Tinyen Shih
#### Executive summary

#### Rationale
Why should anyone care about this question?

The weakest link of any cybersecurity setup today is often the human one, and any algorithmic assistance that can be rendered to help distinguish between safe and dangerous emails enhances overall cybersecurity. Because the point of storing information is the intention to retrieve it later, the one consistent lever attackers can pull is on the coattails of people with legitimate access. This weakness is not something that can be patched away completely, and exploits utilizing the credentials of legitimate users often comes though emails, often refered to as phishing emails.
By exploiting the human mind's tendency to create mental shortcuts when doing routine tasks like reading emails, phishing emails can trick users into using their elevated privileges on a computer or a network to allow the attacker access the same sensitive information. With language models becoming better to write more natural-sounding emails, users' abilities to distinguish a suspicious email are diminished. In light of that, the best way to protect a user from these emails is to never let it get to them in the first place by blocking through spam filters. However, the filters must get better in response to improved attackers, just another cycle of the arms race between attackers and defenders in the cybersecurity space. Without improvements, every entity dealing with sensitive information becomes that much less safe.

#### Research Question
What are you trying to answer?

Can phishing emails be distinguished from legitimate emails reliably? Which classification methods are best at distinguishing between safe and dangerous emails?

#### Data Sources
What data will you use to answer you question?

The CEAS_08.csv file from the following Kaggle link was used for both training and testing data https://www.kaggle.com/datasets/naserabdullahalam/phishing-email-dataset.

#### Methodology
What methods are you using to answer the question?

The message bodies will be tokenized, reduced to root forms, and then combined with other metrics about the metadata of the email, such as the presence of links. Thus processed, the traning data will train a classification model, then test data will be fed in to evaluate how effective the model was. Several different classification models will be tried and evaluated. Because email filters are there to block phishing emails and yet still let through legitimate emails, the metric used for evaluation will be accuracy, aiming to minimize the number of misclassified emails overall. 

#### Results
What did your research find?



#### Next steps
What suggestions do you have for next steps?

There are many possible next steps. Phishing emails often take an urgent tone to give readers less time to consider whether the email is legitimate or not, and in theory, a language processing model evaluating the amount of urgency in a block of text could be used to improve email classification.

Another possible step, which lies outside the scope of the given dataset, is to evaluate on whether the email has an attachment or not. While some phishing emails pretend to be from a legitimate site and asks a user to click on a link and log into a legitimate-looking but fake website in order to capture user credentials, others have attachments, that when clicked on, use the user's credentials to execute a program that compromises the computer the email was opened on. The dataset metadata used in this project did not have any information on attachments and so could not be utilized.

#### Outline of project

- [Link to notebook 1]()


##### Contact and Further Information
Tinyen Shih
[LinkedIn](linkedin.com/in/tinyen-shih)