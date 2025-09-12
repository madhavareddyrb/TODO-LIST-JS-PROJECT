## Todo Project

steps:
1.Get all elemets what we need and assign them with const variables
const todoInput = document.getElementById("todo-input");
const addTaskButton = document.getElementById("add-task-btn");
const todoList = document.getElementById("todo-list");

2.for tasks create an array for all tasks
3.Here logic is everything happens when we click on addTaskButton so add eventliseter for that variable
4.Here when we click taskButton we need to grab that text in input label so here to store that value create an const taskText and value comes from todoInput(todoInput.value.trim()) trim() used to remove any extra spaces
5.Every task must be unique and completed tasks or not so we create an id,text,completed object with  const newTask variable
6.we push that newTasks to our array (tasks)
7.After pushing the TodoInput must be empty so clear input
8.log all tasks to debug crt or wrong
9.Here tasks we gone for every refresh to save tasks we use local storage
10.create a function to saves tasks and render later
11.local storage use setItem method to save or create items and it comes with 2 params(key,value) both must be in strings.
12.Here we use JSON stringfiy method to convert tasks object to string.
13.savetasks() after creating a newTask pushing to the tasks
14.Here is catch that DOM maybe loaded or got error in process so change the whole program to after loading dom.document.addEventListener("DOMContentLoaded", () => {whole code})
14.To render every task one by one we need to cretae a function renderTask(task) and log task.
15. To get or render task localStorage.getItem(tasks) here is a catch that we have stored in json form and to convert from string json format to normal array we use JSON.parse let tasks = JSON.parse(localStorage.getItem("tasks"))|| [];
16.Go to console in browser checks the following steps how its working.For local storage inspect->application->loaclStorage
