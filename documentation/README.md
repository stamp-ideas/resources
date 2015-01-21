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

Crop the image by pressing `C` and `Enter`. The artboard will crop to the selection you made in the previous step. Press `Shift+Alt+Cmd+S` to Save for Web. Note the following suggestions:

#### JPEGs
Use this filetype for high-color photos, or any other photorealistic image. 

#### PNGs

This is what you'll want to use in most cases. smaller amounts of color, few or no gradients, and (most importantly) *text.* **If you have text in an image, use PNGs if at all possible.**

Be sure and compress these using [TinyPNG](https://tinypng.com/), or [ImageOptim](https://imageoptim.com/), which is a Finder extension that lets you optimize batches right from the desktop.
    
---

### Step 7: Save the PSD with the guides you've just made

Make sure you're not about to save over the file on the Agency server, then Press `Cmd+S` to save your PSD into the folder you made on the Development server.

### Step 8: Update and/or write index file with new content.

This is where the bulk of your time will be spent. If you duplicated the folder from a previous job, simply update the `ALT` text, perform a `Find and Replace` on all the job number references so your image links are referring to your new folder, then replace all the old images from the previous job with your newly cropped images from Step # 6.

If you're working from the email template, and there isn't a similar job done in the past, write the `HTML` necessary to build the email. Remember, **tables are the commonly accepted best-practice for building HTML emails.**

Here's a checklist for writing emails:

  [ ] Add/update `ALT` text
  [ ] Add/Update Subject line (Also used in `<title>`)
  [ ] Add/Update `View this Email Online` link (to client server `email` folder)
  [ ] Add/Update Plain Text version
  [ ] Add/Update links provided by AE/AC
  [ ] Explicitly declare width/heights on images
  [ ] Ensure that images use absolute linking (so they don't break in MobileStorm)
  
### Step 9: Upload to client's server

This depends on your editor. If you're using an integrated FTP, such as [Coda](https://panic.com/coda/), just switch to the server side, browse to the client's email folder, and upload the job folder from the Development server.

If you're using Filezilla, it's essentially the same process.

### Step 10: Add to MobileStorm

You won't have many opportunities to go wrong in Mobilestorm, but here's a general idea of what you need to do and/or click:

  1. Create Email Campaign (Custom HTML)
  2. If a client list was specified in the email, choose that here. Otherwise, choose the list with the client's name
  3. Give it a unique name that the AC will recognize [**Standardize name of Campaign**]
  4. For the Target, choose LWTTEST unless otherwise specified
  5. FROM name should match client list (in general)
  6. Click 'Save & Continue'
  7. Use subject you were provided in email
  8. Don't mess with personalized options unless specified
  9. paste the URL into the input field to 'grab HTML'. 
  10. Remove the plain-text comment from the bottom of the HTML version, and paste it into the Plain Text tab.
  11. Make sure all links are checked to be replaced with MobileStorm redirects.
  12. Click 'Continue'.
  13. Make sure the following boxes are checked:
    1. Forward to a Friend
    2. Edit Profile
    3. Click Tracking 
    4. Click Stream Tracking
    5. Whitelist Reminder
    6. DO NOT CLICK SOCIAL NETWORKING OR SHOW EMAIL ONLINE
  14. Double check number of subscribers to make sure you're not sending to actual list (just in case. Should be 22)
  15. Scroll down to '...Or Send to A Test Group'
    1. Send to 'Shawn, Brandon, & Friends' List to test
    2. click 'Save'
  
### Test Emails in Various Clients

Test emails like you would most everything else: check as many clients as reasonably possible. If accessible, testing services like [Litmus](https://litmus.com/) are great tools to speed this up. Otherwise, refer to the Stamp Logins document for these accounts:
- Your Local Outlook (probably 2013)
- Gmail
- Outlook.com
- Yahoo! Mail (it'll probably be off-center. [Here's how to fix it.](https://litmus.com/blog/fixing-table-alignment-in-yahoo-mail))

### Update Web Version with MS Links

Once you've finished testing, replace the links in the web version (the files on the client's server) with MobileStorm links, so they'll get accurate tracking in the Web Version.

### Send Internal Test in MS

Once you've sent tests to various clients, and you've already sent to the `Shawn, Brandon, and Friends` list, send an `Internal Test`. This will send most of the Stamp people a test, and you'll most likely get an edit or two.

### Send Confirmation email to AC (CC AE until told otherwise)

It's generally advised to wait a few minutes before notifying the Account Coordinator that you've finished the email. Otherwise, you might be doing edits after they send a hard-test. (Which messes things up.)

### Stamp Job Jacket and Put in Basket

Stamp the Job Jacket, and put it in the basket.

### Send GIF to John and Taylor about your experience following this guide

![Good Job GIF](http://media.giphy.com/media/wvrn7MMemcOB2/giphy.gif)
  
## Best Practices

These are general 'best practices' for building emails. This is a constantly-updated list.

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