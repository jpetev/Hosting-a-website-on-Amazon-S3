[README.md](https://github.com/user-attachments/files/23135051/README.md)
<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Host a Website on Amazon S3

**Project Link:** [View Project](http://learn.nextwork.org/projects/aws-host-a-website-on-s3)

**Author:** Jaheem Petersen  
**Email:** jaheem5etersen@gmail.com

---

![Image](http://learn.nextwork.org/overjoyed_lavender_smart_tamarillo/uploads/aws-host-a-website-on-s3_5d4474f9)

---

## Introducing Today's Project!

In this project, I will demonstrate how to create an S3 bucket, to store pictures and files. I'm doing this project to learn how to host a website on Amazon S3.

### Tools and concepts

Services I used were the S3 buckets, ACLs, website hosting and bucket policies. Key concepts I learnt included managing ACLs, creating bucket policies and hosting a static website.

### Project reflection

This project took me approximately 45 minutes. The most challenging part was creating the bucket policy, I made an error and had to figure out where I went wrong entering the code. It was most rewarding to publicize my website, by making the index.html file public using ACLs.

---

## How I Set Up an S3 Bucket

Creating an S3 bucket took me 5 minutes, the process was very simple and straight forward.

The Region I picked for my S3 bucket was north virginia, because it's the closest region to my current location out of the regions available.

S3 bucket names are globally unique! This means no other AWS account in the entire world can use my bucket's name.

![Image](http://learn.nextwork.org/overjoyed_lavender_smart_tamarillo/uploads/aws-host-a-website-on-s3_ba6d42ad)

---

## Upload Website Files to S3

### index.html and image assets

I uploaded two files to my S3 bucket - 44 from the unzipped folder, and 1 from the index HTML. The Index HTML file is used to create and design web pages. The folder included my images, which will be used to design the web pages.

Both files are necessary for this project as one indicates where objects are assigned, and the other includes the objects that are going to be used.

![Image](http://learn.nextwork.org/overjoyed_lavender_smart_tamarillo/uploads/aws-host-a-website-on-s3_a265af88)

---

## Static Website Hosting on S3

Website hosting means hosting your website publicly so that it's accessible on the internet.

To enable website hosting with my S3 bucket, I clicked on my bucket from the general purpose buckets tab. From there I choose the properties tab, then edit on the static website hosting panel. Once I was there, I enabled static website hosting, and made sure host a static website was selected as the hosting type. Lastly I enter index.html in the index document line, then I saved my changes.

An ACL is a set of rules that determine who can access a resource. I enabled ACLs, so that i can control who can manage the objects I upload to my bucket.

![Image](http://learn.nextwork.org/overjoyed_lavender_smart_tamarillo/uploads/aws-host-a-website-on-s3_c22c54c0)

---

## Bucket Endpoints

Once static website is enabled, S3 produces a bucket endpoint URL, which is just like a regular website URL. It allows others to visit your S3 bucket files as a wesbite.

When I first visited the bucket endpoint URL, I saw error code '403 Forbidden'. The reason for this error was because my files weren't made public yet, therefore they're not availabl;e to be viewed publicly.

![Image](http://learn.nextwork.org/overjoyed_lavender_smart_tamarillo/uploads/aws-host-a-website-on-s3_22ce4daf)

---

## Success!

To resolve this 403 Forbidden error, I selected the index.html file on the 'Objects' tab. Then I clicked 'Actions', followed by 'make public using ACL' and then 'Make pbulic' at the bottom left. After following those steps, I was able to see my website publicly online.

![Image](http://learn.nextwork.org/overjoyed_lavender_smart_tamarillo/uploads/aws-host-a-website-on-s3_5d4474f9)

---

## Bucket Policies

An alternative to ACLs are bucket policies, which are more advanced compared to ACLs. The benefit of using bucket policies is that it gives you more control than ACLs, while ACLs are useful for managing individual objects within a bucket. ACLs allow different AWS accounts to access and manage files in your bucket.

My bucket policy protects my index.html file from being deleted. I tested this by attempting to delete the file and saw an error saying 'Access denied'.

![Image](http://learn.nextwork.org/overjoyed_lavender_smart_tamarillo/uploads/aws-host-a-website-on-s3_sm2sm2sm)

---

---
