# machinebox-tagbox
Tagbox lets you identify the content of images by getting a list of ordered tags.

* This is a proof-of-concept using Machinebox.io's tagbox for renaming photos with meta data that identifies the content of the images.
* The Docker compose file will also spin up an apache server with a volume (directory) mapped so you can easily feed your photos to tagbox by way of a URL :)

## Setup
1. Clone repo ``git clone https://github.com/seriousfunk/machinebox-tagbox``
2. Create .env file with your Machinebox.io MB_KEY ``echo MB_KEY=YOUR_MB_KEY >> ./.env``
3. Copy your files into the ``images`` folder or update the volume mapping in the docker-compose.yml
4. Start Docker containers ``docker-compose up -d``
5. Tagbox will be running on http://localhost:8888/ and your Apache server on http://localhost:8080/

