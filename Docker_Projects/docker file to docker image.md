 # Create Docker image from Docker file:
 
 Template for Docker file  
 FROM ALPINE (Base image to create new image)
 RUN apt-get install python 
 RUN echo$(pwd)
 RUN touch file.txt
- We can write all these commands in a simple text file to create Docker image.
