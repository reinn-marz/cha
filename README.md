<!doctype html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Absensi SAF</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.8/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-sRIl4kxILFvY47J16cr9ZwB07vP4J8+LH7qKQnuqkuIAvNWLzeN8tE5YBujZqJLB" crossorigin="anonymous">
  </head>
  <body>
    <nav class="navbar navbar-expand-lg bg-body-tertiary">
      <div class="container-fluid">
        <a class="navbar-brand" href="#">Salman Alfarisi Cibinong</a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
          <ul class="navbar-nav me-auto mb-2 mb-lg-0">
            <li class="nav-item">
              <a class="nav-link active" aria-current="page" href="#">Home</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">Link Absensi</a>
            </li>
            <li class="nav-item dropdown">
              <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                Pilihan
              </a>
              <ul class="dropdown-menu">
                <li><a class="dropdown-item" href="#">Kelas 7</a></li>
                <li><a class="dropdown-item" href="#">Kelas 8</a></li>
                <li><a class="dropdown-item" href="#">Kelas 9</a></li>
                <li><hr class="dropdown-divider"></li>
                <li><a class="dropdown-item" href="javascript:void(0);" onclick="window.open('page1.html'); window.open('page2.html');">More</a></li>
              </ul>
            </li>
          </ul>
          <form class="d-flex" role="search">
            <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search"/>
            <button class="btn btn-outline-success rounded-pill" type="submit">Search</button>
          </form>
        </div>
      </div>
    </nav>
    
    <div class="d-flex justify-content-center align-items-center" style="height: 20vh;">
      <div class="text-center">
        <h1>SMP Salman Alfarisi Cibinong</h1>
        <h6 style="margin-top: 20px;">Alamat: Jl. Raya Setu Cikaret, Kp. Kramat RT 02/03, Kelurahan Harapan Jaya, Kecamatan Cibinong, Kabupaten Bogor, Jawa Barat 16914</h6>
      </div>
    </div>
    
    <div class="d-flex justify-content-center align-items-center" style="height: 20vh;">
      <div class="text-center">
        <h2>Daftar Hadir</h2>
        <h6 style="margin-top: 15px;">Date: <span id="currentDate"></span></h6>
      </div>
    </div>

    <div class="card border-primary mb-3" style="max-width: 18rem; margin: 20px auto;">
      <div class="card-header" style="text-align: center;">Kelas-Kelas</div>
      <div class="card-body text-primary">
        <div class="d-grid gap-2">
          <button class="btn btn-danger rounded-pill" onclick="window.location.href='Kelas 7.html';">Kelas 7 - Madinah</button>
          <button class="btn btn-warning rounded-pill" onclick="window.location.href='Kelas 8.html';">Kelas 8 - Arafah</button>
          <button class="btn btn-success rounded-pill" onclick="window.location.href='Kelas 9.html';">Kelas 9 - Mina</button>
        </div>
      </div>
    </div>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.8/dist/js/bootstrap.bundle.min.js" integrity="sha384-FKyoEForCGlyvwx9Hj09JcYn3nv7wiPVlz7YYwJrWVcXK/BmnVDxM+D2scQbITxI" crossorigin="anonymous"></script>
    
    <script>
      const today = new Date();
      const day = String(today.getDate()).padStart(2, '0');
      const month = String(today.getMonth() + 1).padStart(2, '0');
      const year = String(today.getFullYear()).slice(-2);
      const formattedDate = `${day}/${month}/${year}`;
      document.getElementById('currentDate').textContent = formattedDate;
    </script>
  </body>
</html>
