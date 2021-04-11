<template>
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
    <a class="navbar-brand" href="/"><img src="../assets/img/logo.png" alt="Logo"></a>
        <div class="collapse navbar-collapse" id="navbarText">
            <ul class="navbar-nav mr-auto">
                <li class="nav-item active">
                    <a class="nav-link" href="{% url 'patients' %}">Пациенты</a>
                </li>
                <li class="nav-item active">
                    <a class="nav-link" href="{% url 'doctors' %}">Врачи</a>
                </li>
                <li class="nav-item active">
                    <a class="nav-link" href="{% url 'departments' %}">Отделения</a>
                </li>
                <li class="nav-item active">
                    <a class="nav-link" href="{% url 'wards' %}">Палаты</a>
                </li>
                <li class="nav-item active">
                    <a class="nav-link" href="{% url 'add_patient' %}">Новый пациент</a>
                </li>
            </ul>
            <span class="navbar-text">
                <span>Добро пожаловать, {{ user }} | </span>
                <span><a href="{% url 'logout' %}">Выйти</a></span>
            </span>
            <span class="navbar-text">
                <span><a href="{% url 'login' %}">Войти</a></span>
            </span>
        </div>
    </nav>
</template>

<script>
    export default {
        name: 'Nav',
    }
</script>

<style scoped>

</style>