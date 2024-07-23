# r2024_07_23_server_delays

> npm install
> 
> npm start

>> In another terminal
>>   curl http://localhost:3001/hello?data=foobar

In code:
const dispatchAndResetEmail = async () => { 
    console.log("In dispatchAndResetEmail");
    const emails = inputValue.split(',').map(email => email.trim());
    emails.forEach((email) => {
     console.log("Dispatch: ", email );
     var s = fetch("http://localhost:3001/hello?data=" +email  );
     // Note: s is a promise 
   });
