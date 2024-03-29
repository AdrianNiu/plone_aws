# Running Plone on AWS

AWS fargate, a serverless compute engine for containers that works with both ECS and EKS. 

## Build this Presentation

### Build dependencies

- nvm
- pandoc
- bsdtar (part of the `libarchive-tools` package on Ubuntu)

Make sure that your working directory is set up to use the LTS version of node before you begin. Then can just build your
presentation with `make`.

```
$ nvm install --lts
$ make start
```

The Lambda function analyses the input transcript field of the Amazon Lex event. Based on the overall sentiment value, it generates a response message with next step instructions.

GATE an open-source project focus on labeling, processing, benchmarking.

Amazon Comprehend Medical is a HIPAA-eligible natural language processing (NLP) service that uses machine learning to extract health data from medical text–no machine learning experience is required.

Amazon Comprehend can discover the meaning and relationships in text from customer support incidents, product reviews, social media feeds, news articles, documents, and other sources.

brat is an online environment for collaborative text annotation that can be run on a (possibly local) server and then used in a browser. But Annotating significantly longer text spans (i.e. paragraphs) turns out to be really inconvenient.

JS library for ML: Brain.js; Synaptic; Neataptic

text classification is a broad category, various annotation types like product categorization or sentiment annotation are technically just specialized forms of text classification.

sheet query: =QUERY(countries,"SELECT B, D WHERE D > 100000000",1)

The Natural Language Toolkit, or more commonly NLTK, is a suite of libraries and programs for symbolic and statistical natural language processing for English written in the Python programming language. 

RIP Robin Williams（https://zhuanlan.zhihu.com/RIP Robin Williams）

wget --no-check-certificate https://launchpad.net/plone/5.0/5.0.4/+download/Plone-5.0.4-UnifiedInstaller.tgz

Create the JSONL file for Prodigy
Prodigy requires a jsonl file as input data, with a json dictionary per line
prodigy
ner.manual
ner_news_headlines
blank:en
./news_headlines.jsonl
--label PERSON,ORG,PRODUCT,LOCATION


Bidirectional Encoder Representations from Transformers is a Transformer-based machine learning technique for natural language processing pre-training developed by Google.

An Amazon ECS cluster is a logical grouping of tasks or services. We can register one or more Amazon EC2 instances (also referred to as container instances) with our cluster to run tasks on them. 

AWS Fargate, Amazon ECS, Amazon EKS, and AWS Batch make it easy to run and manage Docker containers at scale. AWS Batch provides with a managed batch queue, complete with the ability to specify priority, dependencies, and retries. 

manually set the PORT environment variable. A command like this will work (my preferred option).

PORT=3000 CLIENT_PUBLIC_PATH=http://$C9_HOSTNAME:3001/ RAZZLE_API_PATH=http://$C9_HOSTNAME:3000/api yarn start 

Amazon ECS: Used to deploy an Amazon ECS containerized application as a task set. 

EFS Blobstorage will work with Blobstorage backup with lifecycle rule. AWS VS Azure in storage comparison. 

Extend the Lambda function to identify “hot” topics in the user input even if the sentiment is not negative and take action proactively. 

A basic app or a simple static website will suit for Fargate deployment.

###Under dockerfile to use docker-compose up to run on port 8080.

AWS Fargate platform versions are used to refer to a specific runtime environment for Fargate task infrastructure. It is a combination of the kernel and container runtime versions.

To install the AWS CLI on your Ubuntu-based Lightsail instance, connect to your instance, and type sudo apt-get -y install awscli.

### Correct command for docker run: docker run --rm cloudplone/cms:dev cat /opt/plone/inituser

Be careful of dependency requirement for each plane Colton add ons. 

Amazon EKS integrates Kubernetes with AWS Fargate by using controllers that are built by AWS using the upstream, extensible model provided by Kubernetes.

Kubernetes, written in Go, is inherently multi-arch, providing its control plane components throughout for a number of architectures. In Kubernetes, and by extension in Amazon EKS, the worker node-local supervisor called kubelet instructs the container runtime via a standardized interface to pull container images from a registry such as Amazon ECR and launch them, accordingly. All of which is multi-arch enabled and automated.

A port is an endpoint of communication in an operating system that identifies a specific process or a type of service. Bitnami stacks include several services or servers that require a port.

AWS Ubuntu node version ignore node: adding --ignore-engines

Plone strength: standards conformance, access control, internationalization, aggregation, user-generated content, micro-applications, active user groups and value

NLU takes up the understanding of the data based on grammar, the context in which it was said, and decide on intent and entities.
NLP converts a text into structured data.
NLG generates text based on structured data.

Volto demo website:   https://volto-dev.gptrac.org/
