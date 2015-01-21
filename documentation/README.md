## Email Development

### Step 1: Make a folder on the Development server. (Job code should be name)

When you first get the Job Jacket, make a folder on the Development server with the same name as the Job #. (i.e.: `XX01-XXXX`). This keeps everything organized in the Dev folder, and allows for easy lookup of past jobs.

### Step 2: Duplicate a Similar Job, or the Template

If you've been told there's a similar email that was done in the past (and there probably is), find that job and duplicate the folder. (Update the name to your new Job #.) Check the Job Jacket for any reference number, and that'll probably make it much easier to find the previous job.

### Step 3: Open the PSD and save a copy in the folder you made previously

Go to the Job folder on the `Agency` server, and open the PSD in the `Working` directory. Before you change anything, be sure and `Save As...` into your new folder on the Development server.

### Step 4: Clear Guides on PSD

The artist has probably made a few guides on the document while they were creating it. Since you've saved it as a copy in the previous step, clear all the guides by going to `View > Clear Guides.`

---

Repeat these two steps for every image you'd like to link: 

### Step 5: Make selection + Place Guide(s)

For every image that needs to link somewhere, select the image with the `M` selection tool, and place guides around the selection. This ensures that you're *actually* placing the guides on the edges of the image, because Photoshop allows you to place guides on subpixels, which you can't crop.

### Step 6: Save for Web into images folder

Crop the image by pressing `C` and `Enter`. The artboard will crop to the selection you made in the previous step. Press `Shift+Alt+Cmd+S` to Save for Web. Use the following suggestions:

#### JPEGs
Use this filetype for high-color photos, or any other photorealistic. 

    - Pictures, photos, other high-color images
  - PNG-8 or 24
    - Solid colors, no gradients, TEXT
    
---

### Step 7: Save the PSD with the guides you've just made

### Step 8: Update and/or write index file with new content.
  - Add/update `ALT` text
  - Update Subject line (Also used in `<title>`)
  - Add 'View this Email Online' link (to client server 'email(s)' folder)
  - Update Plain Text version
  - Add/Update links provided by AE/AC
  - Explicitly declare width/heights on images
  - Update images to use absolute linking (so they don't break in MS)
  
### Step 9: Upload to client's server

### Step 10: Add to MobileStorm
  - Create Email Campaign (Custom HTML)
  - If a client list was specified in the email, choose that here. Otherwise, choose the list with the client's name
  - Give it a unique name that the AC will recognize [**Standardize name of Campaign**]
  - For the Target, choose LWTTEST unless otherwise specified
  - FROM name should match client list (in general)
  - Click 'Save & Continue'
  - Use subject you were provided in email
  - Don't mess with personalized options unless specified
  - paste the URL into the input field to 'grab HTML'. 
  - Remove the plain-text comment from the bottom of the HTML version, and paste it into the Plain Text tab.
  - Make sure all links are checked to be replaced with MobileStorm redirects.
  - Click 'Continue'.
  - Make sure the following boxes are checked:
    - Forward to a Friend
    - Edit Profile
    - Click Tracking 
    - Click Stream Tracking
    - Whitelist Reminder
    - DO NOT CLICK SOCIAL NETWORKING OR SHOW EMAIL ONLINE
  - Double check number of subscribers to make sure you're not sending to actual list (just in case. Should be 22)
  - Scroll down to '...Or Send to A Test Group'
    - Send to 'Shawn, Brandon, & Friends' List to test
    - click 'Save'
  
### Test Emails in Various Clients
  - in your local Outlook
  - Gmail
  - Outlook.com
  - Yahoo! Mail

### Update Web Version with MS Links

### Send Internal Test in MS
  - Everyone's going to get this; wait a few minutes to see if anyone has any edits

### Send Confirmation email to AC (CC AE until told otherwise)

### Stamp Job Jacket and Put in Basket

### Send GIF to John and Taylor about your experience following this guide
  
## Best Practices

- Always use tables because 1998
- Escape special characters with their entity code

Linkmap:
- The printout of the email with links drawn on (Amber)


## Resources

### Links

* [Litmus on Animated GIF Usage](https://litmus.com/blog/a-guide-to-animated-gifs-in-email "Litmus Animation Article")
* [Maximum Email Size](http://www.emailonacid.com/blog/details/C13/when_it_comes_to_html_email_size_does_matter "Maximum Email Size")

### Resources

* [Email Testing](http://www.campaignmonitor.com/testing/ "Email Testing")
* [Email Standards Project](http://www.email-standards.org/ "Email Standards Project")
* [Current Browser Support](http://www.email-standards.org/clients/ "Browser Support")
* [Litmus Email Testing](http://litmus.com/email-testing "Litmus Email Testing")
* [Litmus Scope](https://litmus.com/scope/ "Litmus Scope")
* [Campaign Monitor](http://www.campaignmonitor.com/ "Campaign Monitor")
* [CSS Support in Clients](http://www.campaignmonitor.com/css/ "CSS Support")
* [MailChimp](http://mailchimp.com/ "MailChimp")
* [ConstantContact](http://www.constantcontact.com/index.jsp "Constant Contact")