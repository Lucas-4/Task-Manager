<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Task Manager</title>
    <script src="https://kit.fontawesome.com/34bd2298ad.js" crossorigin="anonymous"></script>
    <link rel="icon" href="list-check-solid.png" >
    <style>

        @import url('https://fonts.googleapis.com/css2?family=Roboto&display=swap');
        *{
            font-family: 'Roboto', sans-serif;
            padding: 0;
            margin: 0;
            margin-bottom: 10px;
            box-sizing: border-box;
        }
        .app-container{
            box-shadow: 0px 0px 4px black;
            width: 60%;
            margin-left: auto;
            margin-right: auto;
            padding: 30px;
        }
        ul{
            list-style-type: none;
        }
        i{
            float:right;
            margin-right: 5px;
            cursor: pointer;
        }
        i:hover{
            color: red;
        }
        li{
            border-bottom: solid;
            border-width: 1px;
        }
        .header h1{
            font-size: 30px;
        } 
        .add-task input{
            width: 70%;
            height: 25px;
            border-style: none;
            border-bottom: solid 2px;
            border-color: rgb(0, 184, 98);
            margin-bottom: 2px;
        }
        .add-task input:focus{
            outline: none;
        }
        .add-task button{
            height: 25px;
            display:block;
            padding-left:10px;
            padding-right:10px;
            border-style: none;
            background-color: rgb(0, 184, 98);
            color: white;
            cursor:pointer;
            border-radius: 5px;
            box-shadow: 0px 0px 2px black;
        }
        .add-task button:hover{
            background-color: rgb(4, 155, 84);
        }
        .task-list{
            margin-top: 30px;
        }
        #alert{
            color: red;
            font-size: 11px;
        }
    </style>
</head>
<body>

    <div class="app-container">
        <div class="header">
            <h1>TASK MANAGER</h1>
            <p>Keep track of your life.</p>
        </div>

        <div class="add-task">
            <input type="text" placeholder="Type a task here" id="task-text">
            <p id="alert"></p>
            <button id="add-task-btn">ADD TASK</button>
        </div>

        <div class="task-list">
            <h2>TASK LIST</h2>
            <ul>
            </ul>
        </div>
    </div>
</body>
    <script>
        if(!(localStorage.getItem('tasks')===null)){
            window.onload = displayTaskList;
        }
        let taskArray = new Array;
        
        //function to add a task to local storage
        function addToLocalStorage(){

            //checks if input value is valid
            if(!(document.querySelector('#task-text').value=="" || !(document.querySelector('#task-text').value.trim()))){

                let taskName = document.querySelector('#task-text').value;
                let taskString;
                document.querySelector('#alert').innerText = "";
                //if there isn't a 'tasks' key in local storage, pushes a task to the taskArray and saves it in local storage
                if(localStorage.getItem('tasks')===null){
                    taskArray.push(taskName);
                    taskString = JSON.stringify(taskArray);
                    localStorage.setItem('tasks', taskString);
                } else{ //if a 'tasks' key already exists in local storage, first the taskArray receives the array stored is local storage, and then pushes a task to the taskArray
                    taskArray = JSON.parse(localStorage.getItem('tasks'));
                    taskArray.push(taskName);
                    taskString = JSON.stringify(taskArray);
                    localStorage.setItem('tasks', taskString);
                }
                document.querySelector('#task-text').value = "";
                displayTaskList();
            } else{
                document.querySelector('#alert').innerText = "Invalid task name";
            }
        }

        function displayTaskList(){
            document.querySelector('ul').innerHTML = "";
            taskArray = JSON.parse(localStorage.getItem('tasks'));
            taskArray.forEach(function (task, index){
                let item = document.createElement('li');
                item.appendChild(document.createTextNode(task));
                item.setAttribute('id', index);
                document.querySelector('ul').appendChild(item);
                let icon = document.createElement('i');
                icon.setAttribute('class', 'fa-solid fa-trash-can');
                let li = document.querySelectorAll('li');
                li.forEach(function (list){
                    list.appendChild(icon);
                    list.querySelector('i').addEventListener('click', deleteFromLocalStorage);
                });
            })
        }

        function deleteFromLocalStorage(e){
            if(!(localStorage.getItem('tasks')===null)){
                let id = parseInt(e.target.parentElement.id);
                taskArray = JSON.parse(localStorage.getItem('tasks'));
                taskArray.splice(id, 1);
                let taskString = JSON.stringify(taskArray);
                localStorage.setItem('tasks', taskString);
                displayTaskList();
            }
        }
        
        document.querySelector('#add-task-btn').addEventListener('click', addToLocalStorage);
    </script>
</html>
