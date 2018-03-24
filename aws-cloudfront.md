## Configuring CloudFront for a Static S3 Website

- Got to CloudFront

    ![image](./images/37713068-a8e77b16-2d0d-11e8-90b0-810d4ec4d7bd.png)

- Create a Distribution

    ![image](./images/37713094-baee4858-2d0d-11e8-937b-b31753cc8f91.png)

- Select Web

    ![image](./images/37713114-c877ed58-2d0d-11e8-8f56-310ecba341bd.png)

- Set the `Origin Domain name` to the url of your bucket's static website

- Add your domain to `Alternate Domain Names (CNAMEs)`

    ![image](./images/37713620-5b250a7c-2d0f-11e8-9747-db7d11c956a8.png)

- (bonus) Comment your website's domain so that it's easy to find latter

    ![image](./images/1.png)

- Create it!

    ![image](./images/2.png)

- Select it from the list

    ![image](./images/3.png)

- Go to Error Pages and Create a Custom Error Response

    ![image](./images/4.png)

    This is recommended since static websites return a 404 on all routes except for '/'.
    It will still work fine without this, but crawlers and techy clients might notice

- Edit your error response to look like this

    ![image](./images/5.png)
