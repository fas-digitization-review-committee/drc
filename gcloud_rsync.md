---
title: "Google Cloud commands"
categories: "web dev"
tags: ["Google", "cloud", "git", "github"]
---

## Google Cloud commands

From: ```c:\Users\comstock\OneDrive - Harvard University\programming\osprey>```

	gcloud auth login

	gcloud config set project project-comstock-cc

	gcloud config set project crosseyedcrafts-206710

	gsutil rsync -d -r ./public gs://comstock.cc/bill/ ; gsutil acl -r ch -u AllUsers:R gs://comstock.cc/bill

	gsutil rsync -d -r ./public gs://imaging-services-html/scanCafe/

	gsutil rsync -d -r ./public gs://comstock.cc/bhp/

	gsutil rsync -d -r ./public gs://comstock.cc/preserve-images/

	gsutil rsync -d -r ./public gs://comstock.cc/preserve-images/ ; gsutil acl -r ch -u AllUsers:R gs://comstock.cc/

	gsutil rsync -d -r ./public gs://comstock.cc/barcodeCoversheets/ ; gsutil acl -r ch -u AllUsers:R gs://comstock.cc/

	gsutil rsync -d -r ./public gs://handwriting_recognition/ ; gsutil acl -r ch -u AllUsers:R gs://handwriting_recognition/

	gsutil ls

---

	gsutil acl -r ch -u AllUsers:R gs://comstock.cc/bill

	gsutil acl -r ch -u AllUsers:R gs://comstock.cc/

	gsutil acl -r ch -u AllUsers:R gs://imaging-services-html/scanCafe/

---
	gsutil web set -m index.html -e 404.html gs://comstock.cc/

	gsutil web set -m index.html -e 404.html gs://crosseyedcrafts.com/

	gsutil web set -m index.html -e 404.html gs://imaging-services-html/scanCafe/

---

gcloud ml vision detect-document "gs://handwriting_recognition/*
---

[Google Cloud shell examples](https://cloud.google.com/shell/docs/examples)

# Create a Cloud Storage bucket
gsutil mb gs://my-bucket-555

# Upload some data to the Cloud Storage bucket you created
gsutil cp test.dat gs://my-bucket-555
## Git commands

	git remote -v # shows which external (github) repositories are linked

	git remote add origin https://github.com/comstock/barcodeCoversheets.git

	git push origin master

	 git remote remove origin

[https://storage.googleapis.com/imaging-services-html/scanCafe/index.html](https://storage.googleapis.com/imaging-services-html/scanCafe/index.html)
