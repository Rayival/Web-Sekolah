<template>
    <div class="header">
    <div class="title">
        <img src="~/assets/LOGO-SMK4.png" alt="logo SMKN 4" width="50"/>
            <h1> SMKN 4 Tasikmalaya</h1>
    </div>
    </div>
        <!-- <nav class="navbar navbar-expand-lg bg-body-tertiary">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">Navbar</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav me-auto mb-2 mb-lg-0">
        <li class="nav-item">
          <a class="nav-link active" aria-current="page" href="#">Home</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Link</a>
        </li>
        <li class="nav-item dropdown">
          <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
            Dropdown
          </a>
          <ul class="dropdown-menu">
            <li><a class="dropdown-item" href="#">Action</a></li>
            <li><a class="dropdown-item" href="#">Another action</a></li>
            <li><hr class="dropdown-divider"></li>
            <li><a class="dropdown-item" href="#">Something else here</a></li>
          </ul>
        </li>
        <li class="nav-item">
          <a class="nav-link disabled" aria-disabled="true">Disabled</a>
        </li>
      </ul>
    </div>
  </div>
</nav> -->
        <div class="nav">
            <a href="#">HOME</a>
            <a href="#">PROFIL<i class="fas fa-caret-down"></i></a>
            <a href="#">KURIKULUM<i class="fas fa-caret-down"></i></a>
            <a href="#">SAPRAS</a>
            <a href="#">EKSTRAKURIKULER</a>
            <a href="#">ARTIKEL</a>
            <a href="#">AGENDA</a>
            <a href="#">ALUMNI<i class="fas fa-caret-down"></i></a>
        </div>
</template>
  
  <style scoped>
        .header {
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 10px 20px;
            border-bottom: 1px solid #e0e0e0;
        }
        .header img {
            height: 50px;
        }
        .header .title {
            display: flex;
            align-items: center;
        }
        .header .title h1 {
            margin: 0 0 0 10px;
            font-size: 24px;
            color: #000000;
        }
        .nav {
            display: flex;
            justify-content: center;
            padding: 10px 0;
            background-color: #0365AE;
        }
        .nav a {
            margin: 0 15px;
            text-decoration: none;
            color: #ffffff;
            font-size: 14px;
        }
        .nav a:hover {
            text-decoration: underline;
        }
  </style>
