<div align="center">
  
# JavaScript

## 21 days coding challenge by _Lighthouse Labs_
  
### Completed one challenge a day from _November 22_ until _December 12_ to develop a daily coding habit.
 ___________________________________________________________________________________________________________________

| <a href="#C1">_Challenge 1_</a> | <a href="#C2">_Challenge 2_</a> | <a href="#C3">_Challenge 3_</a> | <a href="#C4">_Challenge 4_</a> | <a href="#C5">_Challenge 5_</a> | <a href="#C6">_Challenge 6_</a> | <a href="#C7">_Challenge 7_</a> | <a href="#C8">_Challenge 8_</a> | <a href="#C9">_Challenge 9_</a> | <a href="#C10">_Challenge 10_</a> | <a href="#C11">_Challenge 11_</a> | <a href="#C12">_Challenge 12_</a> | <a href="#C13">_Challenge 13_</a> | <a href="#C14">_Challenge 14_</a> | <a href="#C15">_Challenge 15_</a> | <a href="#C16">_Challenge 16_</a> | <a href="#C17">_Challenge 17_</a> | <a href="#C18">_Challenge 18_</a> | <a href="#C19">_Challenge 19_</a> | <a href="#C20">_Challenge 20_</a> | <a href="#C21">_Challenge 21_</a> |
  
![image](https://user-images.githubusercontent.com/91167955/147256637-ab322ac9-fa73-4970-a690-4f227cbea940.png)
___________________________________________________________________________________________________________________

<h2 id="C1"> ⭐ Challenge 1 </h2>
  
<img src="https://user-images.githubusercontent.com/91167955/147261441-33f716e8-b166-43f1-8678-e5e4d0f415b1.png" width="45%" height="30%">

### ✔️ _Solution_
  ``` Javascript
  const parseMessage = (origin, message) => {
  return origin + ": " + message;
}
  ```
___________________________________________________________________________________________________________________
  
<h2 id="C2"> ⭐ Challenge 2</h2>  
 
<img src="https://user-images.githubusercontent.com/91167955/147267407-c50000c8-d6c8-4919-a8a3-1893cd934e37.png" width="45%" height="30%"> 

 
### ✔️ _Solution_
  ``` Javascript
  const generateAstronautTag = (astronaut) => {
  return astronaut.prefix + ": " +  astronaut.firstName + " \"" + astronaut.nickname + "\" " + astronaut.lastName;
}
  ```
___________________________________________________________________________________________________________________

<h2 id="C3"> ⭐ Challenge 3</h2>  
 
<img src="https://user-images.githubusercontent.com/91167955/147270249-7a6ad422-05ec-46de-804a-cb19d7afee6f.png" width="45%" height="30%"> 

### ✔️ _Solution_
  ``` Javascript

const checkGaugeStatus = (gauge) => {

  if(gauge.current>=gauge.min && gauge.current <= gauge.max){
    
    return true;
    
  }else{
    
    return false;

  }
}
  ```
___________________________________________________________________________________________________________________
          
<h2 id="C4"> ⭐ Challenge 4</h2>  
 
<img src="https://user-images.githubusercontent.com/91167955/147272036-eb552ec2-1c1d-4fd8-a0a5-b69cc1d7447e.png" width="45%" height="30%"> 

### ✔️ _Solution_
  ``` Javascript
const switchToggle = (toggle) => {
  toggle.isOn = !toggle.isOn;
  return toggle;
}
  ```
___________________________________________________________________________________________________________________

<h2 id="C5"> ⭐ Challenge 5</h2>  
 
<img src="https://user-images.githubusercontent.com/91167955/147272277-f8f54198-4e4e-417c-bc80-8cac5872474a.png" width="45%" height="30%"> 

### ✔️ _Solution_
  ``` Javascript
const addJobToAstronaut = (astronaut, job) => {
  astronaut.job = job;
  return astronaut;
}
  ```
___________________________________________________________________________________________________________________

<h2 id="C6"> ⭐ Challenge 6</h2>  
 
<img src="https://user-images.githubusercontent.com/91167955/147272586-81fca819-d697-411e-8435-b33f59af86ad.png" width="45%" height="30%"> 

### ✔️ _Solution_
  ``` Javascript
const addAstronautToRoster = (roster, astronaut) => {
  roster.push(astronaut);
  return roster;
}
  ```
___________________________________________________________________________________________________________________

<h2 id="C7"> ⭐ Challenge 7</h2>  
 
<img src="https://user-images.githubusercontent.com/91167955/147273185-0bfad829-00ea-43ec-80c7-d1834e132ad3.png" width="45%" height="30%"> 

### ✔️ _Solution_
  ``` Javascript
const storeWeatherConditions = (temperature, condition, windSpeed, windDirection) => {

  newTemperature = Math.round((temperature - 32)/1.8);
  newWindSpeed = Math.round(windSpeed*0.44704);
  
  const structure = {
    temperature:newTemperature, 
    condition:condition,
    windSpeed:newWindSpeed, 
    windDirection:windDirection,
  }
  return structure;
}
  ```
___________________________________________________________________________________________________________________

<h2 id="C8"> ⭐ Challenge 8</h2>  
 
<img src="https://user-images.githubusercontent.com/91167955/147273419-41fd3198-a3ce-456e-ab30-c6f564143a33.png" width="45%" height="30%"> 

### ✔️ _Solution_
  ``` Javascript
const countActiveAstronauts = (roster) => {
  var count = 0;
  
  for(i=0; i<roster.length; i++){
    count++;
  }
  return count;
}
  ```
___________________________________________________________________________________________________________________

<h2 id="C9"> ⭐ Challenge 9</h2>  
 
<img src="https://user-images.githubusercontent.com/91167955/147273654-cef1cbaa-41d4-4f6e-8c91-ca02278b7ef3.png" width="45%" height="30%"> 

### ✔️ _Solution_
  ``` Javascript
const listAstronautJobs = (roster) => {
  var arr = [];
  
  for(i = 0; i < roster.length; i++){
    arr.push(roster[i].job);
  }
  return arr;
}
  ```
___________________________________________________________________________________________________________________

<h2 id="C10"> ⭐ Challenge 10</h2>  
 
<img src="https://user-images.githubusercontent.com/91167955/147273803-f5b3748d-dee2-4f43-a579-c9f6bc515409.png" width="45%" height="30%"> 

### ✔️ _Solution_
  ``` Javascript
const averageWindSpeed = (weatherEntries) => {
  var count = 0;
  var sum = 0;
  
  for(i=0; i<weatherEntries.length; i++){
    sum += weatherEntries[i].windSpeed;
    count++;
  }
  return Math.round(sum/count);
}
  ```
___________________________________________________________________________________________________________________

<h2 id="C11"> ⭐ Challenge 11</h2>  
 
<img src="https://user-images.githubusercontent.com/91167955/147273965-e108f37a-0c6f-4e49-a0ac-4468cb87c0ad.png" width="45%" height="30%"> 

### ✔️ _Solution_
  ``` Javascript
const bookFreePlatform = (platformList, missionDate) => {
  for(i=0; i<platformList.length; i++){
    if(platformList[i].bookDate === undefined){
      platformList[i].bookDate = missionDate;
      break;
    }
  }
  return platformList;
}
  ```
___________________________________________________________________________________________________________________

<h2 id="C12"> ⭐ Challenge 12</h2>  
 
<img src="https://user-images.githubusercontent.com/91167955/147274088-7fb75f41-eaa1-4af0-b541-b39af2c62f7e.png" width="45%" height="30%"> 

### ✔️ _Solution_
  ``` Javascript
const parseTranscripts = (messages) => {
  var arr = [];
  var result = "";
  
  for(i=0; i<messages.length; i++){
    result = messages[i].origin + ": " + messages[i].message;
    arr.push(result);
  }
  return arr;
}
  ```
___________________________________________________________________________________________________________________

<h2 id="C13"> ⭐ Challenge 13</h2>  
 
<img src="https://user-images.githubusercontent.com/91167955/147274241-afafc2c7-68bb-49d8-983d-05229cf2fee9.png" width="45%" height="30%"> 

### ✔️ _Solution_
  ``` Javascript
const checkAllGauges = (gaugeList) => {
  
  var result = true;
  
  for(i=0; i<gaugeList.length; i++){

    if(gaugeList[i].current < gaugeList[i].min ||
    gaugeList[i].current > gaugeList[i].max){
      result = false;
      
    }
  }
  return result;
}
  ```
___________________________________________________________________________________________________________________

<h2 id="C14"> ⭐ Challenge 14</h2>  
 
<img src="https://user-images.githubusercontent.com/91167955/147274437-1a801a49-e31f-471b-be17-3a5077158dd2.png" width="45%" height="30%"> 

### ✔️ _Solution_
  ``` Javascript
const switchAllTogglesOn = (toggleList) => {
  for(i=0; i<toggleList.length; i++){
    toggleList[i].isOn = true;
  }
  return toggleList;
}
  ```
___________________________________________________________________________________________________________________

<h2 id="C15"> ⭐ Challenge 15</h2>  
 
<img src="https://user-images.githubusercontent.com/91167955/147274577-7472e8f0-f42c-4f07-b57d-cf371b20bfd7.png" width="45%" height="30%"> 

### ✔️ _Solution_
  ``` Javascript
const timeRemaining = (launchDate, missionName, fakeToday) => {
  const today = fakeToday || new Date()
  const firstDate = new Date(launchDate);
  const secondDate = new Date(today);
  const diffDays = Math.round(Math.abs((firstDate - secondDate) / (24 * 60 * 60 * 1000)));
  
  return {missionName : missionName,
    daysRemaining : diffDays
  }
}
  ```
___________________________________________________________________________________________________________________

<h2 id="C16"> ⭐ Challenge 16</h2>  
 
<img src="https://user-images.githubusercontent.com/91167955/147274717-e0d5e6c0-df6c-418f-9991-31adb02e6644.png" width="45%" height="30%"> 

### ✔️ _Solution_
  ``` Javascript
const getAverageSpeed = (firstPosition, secondPosition) => {
  distance = secondPosition.altitude - firstPosition.altitude;
  time = secondPosition.time - firstPosition.time;
  speed = distance/time;
  return parseFloat(speed.toFixed(1));
}
  ```
___________________________________________________________________________________________________________________

<h2 id="C17"> ⭐ Challenge 17</h2>  
 
<img src="https://user-images.githubusercontent.com/91167955/147279925-10b06ea5-1587-42c6-874b-e98358eb882a.png" width="45%" height="30%"> 

### ✔️ _Solution_
  ``` Javascript
const switchSpecificToggle = (toggleList, specificToggle) => {
    for(i=0; i<toggleList.length; i++){
      if(toggleList[i].name == specificToggle){
        toggleList[i].isOn = true;
      }
    }
  return toggleList;
}
  ```
___________________________________________________________________________________________________________________

<h2 id="C18"> ⭐ Challenge 18</h2>  
 
<img src="https://user-images.githubusercontent.com/91167955/147280099-f68ca98c-9330-416d-941b-503669bc105d.png" width="45%" height="30%"> 

### ✔️ _Solution_
  ``` Javascript
const chooseLunchWinner = (listOfChoices) => {

  var cnt1 = 0;
  var cnt2 = 0;
  var first = listOfChoices[0];
  
  for(i=0; i<listOfChoices.length; i++){
    if(listOfChoices[i] == first){
      cnt1++;
    }else{
      second = listOfChoices[i];
      cnt2++;
    }
  }
  
  if(cnt1>cnt2){
    return first;
  }else{
    return second;
  }
}
  ```
___________________________________________________________________________________________________________________

<h2 id="C19"> ⭐ Challenge 19</h2>  
 
<img src="https://user-images.githubusercontent.com/91167955/147280282-7491c22b-d4e5-452c-9cc5-48d7e4b35436.png" width="45%" height="30%"> 

### ✔️ _Solution_
  ``` Javascript

const organizeData = (receivedData) => {
  var arr = [];
  
for(i=0; i<receivedData.length; i++){
  arr.push(receivedData[i].type)
}

var newArr = arr.filter((value, index) => arr.indexOf(value) === index);

var obj = {};

for(i=0; i<newArr.length; i++){
  var valueArr = [];
  
for(j=0; j<receivedData.length; j++){
    if(newArr[i] == receivedData[j].type){
      valueArr.push(receivedData[j].data);
      obj[newArr[i]] = valueArr;
    }
}
}
return obj;
}
  ```
___________________________________________________________________________________________________________________

<h2 id="C20"> ⭐ Challenge 20</h2>  
 
<img src="https://user-images.githubusercontent.com/91167955/147281561-3f78b2f2-bfb1-48ef-8f56-0d54f8c830a4.png" width="45%" height="30%"> 

### ✔️ _Solution_
  ``` Javascript
const confirmReentryPlans = (speed, missionData, checks) => {

if(speed > checks.maxSpeed || speed < checks.minSpeed){
  return false;
}

for(const key in missionData){
  const check_key_length = checks.dataEntries[key];
  const key_length = missionData[key].length;
  
  if(key_length != check_key_length){
    return false;
  }
}
return true;
}
  ```
___________________________________________________________________________________________________________________

<h2 id="C21"> ⭐ Challenge 21</h2>  
 
<img src="https://user-images.githubusercontent.com/91167955/147281794-8b266596-cd33-40fd-a565-6d2cec1f3305.png" width="45%" height="30%"> 

### ✔️ _Solution_
  ``` Javascript
const parseMissionSummary = (exchanges, missionData) => {

  var arr = [];
  
  for(i=0; i<exchanges.length; i++){
    var str = exchanges[i].origin + ": " + exchanges[i].message;
    arr.push(str);
  }
  
  var obj = {};
  obj.transcript = arr;
  obj.missionData = missionData;
  return obj;
}
  ```
 __________________________________________________________________________________________________________________

</div>

