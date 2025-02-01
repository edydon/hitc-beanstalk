# Sets the Base Image for subsequent instructions. 
FROM  python:3.11-slim

# Sets the working directory (image) for any subsequent RUN, CMD and COPY instruction 
WORKDIR  /app


# Copies files or directories from the host into the image
COPY  .  /app


# Image build step

# The state of the container after a RUN command 
# will be committed to the container image

# Do not save downloaded packages locally - 
# useful only if pip was going to re-install the same packages
RUN  pip  --no-cache-dir install   -r  requirements.txt

EXPOSE  3000

CMD  [ "python", "app.py" ]
