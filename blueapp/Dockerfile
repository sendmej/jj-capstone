FROM python:3.7.3-stretch

WORKDIR /jjcapstone

## Step 2:
COPY . blueapp.py /jjcapstone/

## Step 3:
# Install packages from requirements.txt
# hadolint ignore=DL3013
RUN pip install --upgrade pip &&\
    pip install --trusted-host pypi.python.org -r requirements.txt

## Step 4:
# Expose port 80
EXPOSE 5000

## Step 5:
# Run app.py at container launch

CMD ["python", "blueapp.py"] 