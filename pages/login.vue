<template>
<html lang="ru">
<head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link href="https://unpkg.com/tailwindcss@2.0.3/dist/tailwind.min.css" rel="stylesheet">
    <link href="https://unpkg.com/tailwindcss/dist/tailwind.min.css" rel="stylesheet"/>
    <link href="https://unpkg.com/@tailwindcss/custom-forms/dist/custom-forms.min.css" rel="stylesheet"/>
    <link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">
</head>

<body class="bg-gray-50">
<div class="flex items-center min-h-screen bg-gray-50 dark:bg-gray-900">
    <div class="container mx-auto">
        <button class="select-none w-full text-md text-center text-gray-400 hover:text-purple-800 font-bold"><NuxtLink to="/"><h2 >Вернуться на главную</h2></NuxtLink></button>
        <div class="max-w-md mx-auto my-4 bg-white p-5 rounded-xl shadow-lg">
            <div class="text-center">
                <h1 class="my-3 text-3xl font-semibold text-gray-700 dark:text-gray-200">Авторизация</h1>
                <p class="text-gray-400 dark:text-gray-400">Войдите в профиль чтобы продолжить</p>
            </div>
            <div class="m-7">
                <form action="https://api.web3forms.com/submit" method="POST" id="form">

                    <input type="hidden" name="apikey" value="YOUR_ACCESS_KEY_HERE">
                    <input type="hidden" name="subject" value="New Submission from Web3Forms">
                    <input type="checkbox" name="botcheck" id="" style="display: none;">


                    <div class="mb-6">
                        <label for="name" class="block mb-2 text-sm text-gray-600 dark:text-gray-400">Почтовый адрес</label>
                        <input type="text" name="name" id="name" placeholder="Введите имя и фамилию" required class="w-full px-3 py-2 placeholder-gray-300 border border-gray-300 rounded-md focus:outline-none focus:ring focus:ring-indigo-100 focus:border-indigo-300 dark:bg-gray-700 dark:text-white dark:placeholder-gray-500 dark:border-gray-600 dark:focus:ring-gray-900 dark:focus:border-gray-500" />
                    </div>
                    <div class="mb-6">
                        <label for="message" class="block mb-2 text-sm text-gray-600 dark:text-gray-400">Пароль</label>
                        <input type="text" name="phone" id="phone" placeholder="Введите пароль" required class="w-full px-3 py-2 placeholder-gray-300 border border-gray-300 rounded-md focus:outline-none focus:ring focus:ring-indigo-100 focus:border-indigo-300 dark:bg-gray-700 dark:text-white dark:placeholder-gray-500 dark:border-gray-600 dark:focus:ring-gray-900 dark:focus:border-gray-500" />
                    </div>
                    <div class="mb-6">
                        <button type="submit" class="w-full px-3 py-4 hover:text-gray-200 hover:bg-gray-800 bg-purple-800 mx-auto lg:mx-0 gradient2 text-white rounded-xl py-4 px-8 shadow-xl transform hover:scale-105 transition delay-50 duration-300 ease-in-out">Войти</button>
                    </div>
                    <p class="text-base text-center text-gray-400" id="result">
                    </p>
                    <button class="select-none w-full text-1xl text-center text-black hover:text-purple-800"><NuxtLink to="/registration"><h2 >Нет аккаунта?</h2></NuxtLink></button>
                </form>
            </div>
            
        </div>
        
    </div>
</div>
</body>
</html>

</template>

<script>

</script>

<style scoped>

       .topnav{
       background-color: rgb(10, 10, 10);
      }

      .browser-mockup {
        border-top: 2em solid rgba(230, 230, 230, 0.7);
        position: relative;
        height: 60vh;
      }
    
</style>
