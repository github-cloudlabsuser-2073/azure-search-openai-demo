
# Backend Application Documentation
The backend application is responsible for handling the core logic of the application. It interacts with Azure Search and OpenAI APIs to perform semantic search and generate embeddings for text and images.
## Directory Structure
•	app/backend/: This is the root directory of the backend application.
•	approaches/: This directory contains different approaches to perform the search.
•	approach.py: This Python file contains the core logic for the search functionality.
•	README.md: This file contains the documentation for the backend application.
## Core Components
approach.py
This Python file contains the core logic for the search functionality of the application.
### Classes
•	Document: Represents a document in the search index.
•	ThoughtStep: Represents a step in the thought process.
•	Approach: Abstract base class representing an approach to perform the search.
### Methods
•	build_filter: Builds a filter for the search.
•	search: Performs the search using the Azure Search API.
•	get_sources_content: Gets the content of the sources.
•	get_citation: Gets the citation for a source.
•	compute_text_embedding: Computes the text embedding using the OpenAI API.
•	compute_image_embedding: Computes the image embedding using the Azure Computer Vision API.
•	run: Abstract method meant to be implemented by subclasses of the Approach class.
## How to Run
To run the backend application, navigate to the app/backend/ directory and run the following command:
´python main.py´

# Requirements 
The backend application requires the following Python packages:
•	aiofiles==23.2.1
•	aiohttp==3.9.5
•	aiosignal==1.3.1
•	annotated-types==0.6.0
•	anyio==4.3.0
•	asgiref==3.8.1
•	attrs==23.2.0
•	azure-ai-documentintelligence==1.0.0b3
•	azure-common==1.1.28
•	azure-core==1.30.1
•	azure-core-tracing-opentelemetry==1.0.0b11
•	azure-identity==1.16.0
•	azure-monitor-opentelemetry==1.4.2
•	azure-monitor-opentelemetry-exporter==1.0.0b25
•	azure-search-documents==11.6.0b1
•	azure-storage-blob==12.20.0
•	azure-storage-file-datalake==12.15.0
•	beautifulsoup4==4.12.3
•	blinker==1.8.2
•	certifi==2024.2.2
•	cffi==1.16.0
•	charset-normalizer==3.3.2
•	click==8.1.7
•	cryptography==42.0.7
•	deprecated==1.2.14
•	distro==1.9.0
•	ecdsa==0.19.0
•	fixedint==0.1.6
•	flask==3.0.3
•	frozenlist==1.4.1
•	h11==0.14.0
•	h2==4.1.0
•	hpack==4.0.0
•	httpcore==1.0.5
•	httpx[http2]==0.27.0
•	hypercorn==0.16.0
•	hyperframe==6.0.1
•	idna==3.7
•	importlib-metadata==7.0.0
•	isodate==0.6.1
•	itsdangerous==2.2.0
•	jinja2==3.1.4
•	markupsafe==2.1.5
•	microsoft-kiota-abstractions==1.3.2
•	microsoft-kiota-authentication-azure==1.0.0
•	microsoft-kiota-http==1.3.1
•	microsoft-kiota-serialization-json==1.2.0
•	microsoft-kiota-serialization-text==1.0.0
•	msal==1.28.0
•	msal-extensions==1.1.0
•	msgraph-core==1.0.0
•	msgraph-sdk==1.1.0
•	msrest==0.7.1
•	multidict==6.0.5
•	numpy==1.26.4
•	oauthlib==3.2.2
•	openai[datalib]==1.30.1
•	openai-messages-token-helper==0.1.4
•	opentelemetry-api==1.24.0
•	opentelemetry-instrumentation==0.45b0
•	opentelemetry-instrumentation-aiohttp-client==0.45b0
•	opentelemetry-instrumentation-asgi==0.45b0
•	opentelemetry-instrumentation-dbapi==0.45b0
•	opentelemetry-instrumentation-django==0.45b0
•	opentelemetry-instrumentation-fastapi==0.45b0
•	opentelemetry-instrumentation-flask==0.45b0
•	opentelemetry-instrumentation-httpx==0.45b0
•	opentelemetry-instrumentation-openai==0.18.2
•	opentelemetry-instrumentation-psycopg2==0.45b0
•	opentelemetry-instrumentation-requests==0.45b0
•	opentelemetry-instrumentation-urllib==0.45b0
•	opentelemetry-instrumentation-urllib3==0.45b0
•	opentelemetry-instrumentation-wsgi==0.45b0
•	opentelemetry-resource-detector-azure==0.1.5
•	opentelemetry-sdk==1.24.0
•	opentelemetry-semantic-conventions==0.45b0
•	opentelemetry-semantic-conventions-ai==0.2.0
•	opentelemetry-util-http==0.45b0
•	packaging==24.0
•	pandas==2.2.2
•	pandas-stubs==2.2.2.240514
•	pendulum==3.0.0
•	pillow==10.3.0
•	portalocker==2.8.2
•	priority==2.0.0
•	psutil==5.9.8
•	pyasn1==0.6.0
•	pycparser==2.22
•	pydantic==2.7.1
•	pydantic-core==2.18.2
•	pyjwt[crypto]==2.8.0
•	pymupdf==1.24.4
•	pymupdfb==1.24.3
•	pypdf==4.2.0
•	python-dateutil==2.9.0.post0
•	python-jose[cryptography]==3.3.0
•	pytz==2024.1
•	quart==0.19.5
•	quart-cors==0.7.0
•	regex==2024.5.15
•	requests==2.31.0
•	requests-oauthlib==2.0.0
•	rsa==4.9
•	six==1.16.0
•	sniffio==1.3.1
•	soupsieve==2.5
•	std-uritemplate==0.0.57
•	tenacity==8.3.0
•	tiktoken==0.7.0
•	time-machine==2.14.1
•	tqdm==4.66.4
•	types-beautifulsoup4==4.12.0.20240511
•	types-html5lib==1.1.11.20240228
•	types-pillow==10.2.0.20240511
•	types-pyasn1==0.6.0.20240402
•	types-python-jose==3.3.4.20240106
•	types-pytz==2024.1.0.20240417
•	typing-extensions==4.11.0
•	tzdata==2024.1
•	urllib3==2.2.1
•	uvicorn==0.29.0
•	werkzeug==3.0.3
•	wrapt==1.16.0
•	wsproto==1.2.0
•	yarl==1.9.4
•	zipp==3.18.2







