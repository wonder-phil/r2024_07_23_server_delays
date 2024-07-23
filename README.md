# r2024_07_23_server_delays

> npm install
> 
> npm start

>> In another terminal
>>  term>  curl http://localhost:3001/hello?data=foobar

## In code:
```
 const dispatchAndResetEmail = async () => { 
    console.log("In dispatchAndResetEmail");
    const emails = inputValue.split(',').map(email => email.trim());
    setInputValue("");
    emails.forEach((email) => {
     console.log("Dispatch: ", email );
     var s = fetch("http://localhost:3001/hello?data=" +email  );
     // Note: s is a promise 
  });
```

Test by entering: 
1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48,49,
