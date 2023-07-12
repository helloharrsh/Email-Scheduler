# Email-Scheduler
This Node.js-based automated email scheduler integrates with the Sendinblue API, allowing users to schedule and send emails at specific dates and times. With customizable email templates and recipient selection, it's a convenient solution for automating email communication and saving time.

# Prerequisites:

  -> Node.js (version 12 or above)
  
  -> NPM (version 6 or above)
  
  -> Sendinblue account and API key
  
# Getting started: 

  -> Clone the repository and install dependencies:
  
  -> `git clone https://github.com/yourusername/automated-email-scheduler.git`

  -> `cd automated-email-scheduler`
  
  -> `npm install`

  -> Set up the environment variables: Create a `.env` file in the root of the project and add the following variables:
  
     `SENDINBLUE_API_KEY=your_sendinblue_api_key`
     
     `EMAIL_FROM=your_email_address`
     
     `EMAIL_TO=recipient_email_address`
     
  -> Set up the email template: Create an `HTML` file in the templates directory with your email content.

  -> Set up the schedule: In the `index.js` file, set up the cron schedule using the Node Cron syntax. 
  -> `For example:`
  
    `cron.schedule('* * * * *', () => {
        sendEmail();
       });`
       
  -> This will send the email every minute.

  -> Run the application: `npm start`.
  
# License:

  -> This project is licensed under the MIT License.
