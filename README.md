<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Sign Up</title>

    <!-- Bootstrap CSS -->
    <link 
        href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" 
        rel="stylesheet"
    >

    <!-- Our Group CSS -->
    <link rel="stylesheet" href="style.css">
</head>

<body>

    <!-- Navigation -->
    <nav class="navbar navbar-expand-lg bg-dark navbar-dark">
        <div class="container">
            <a class="navbar-brand" href="index.html">Group 11</a>

            <button 
                class="navbar-toggler" 
                type="button" 
                data-bs-toggle="collapse" 
                data-bs-target="#navbarNav"
            >
                <span class="navbar-toggler-icon"></span>
            </button>

            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto">
                    <li class="nav-item">
                        <a class="nav-link" href="index.html">Home</a>
                    </li>

                    <li class="nav-item">
                        <a class="nav-link active" href="signup.html">Sign Up</a>
                    </li>
                </ul>
            </div>
        </div>
    </nav>


    <!-- Sign Up Form -->
    <div class="container mt-5 mb-5">

        <div class="row justify-content-center">

            <div class="col-md-8 col-lg-6">

                <div class="card shadow">

                    <div class="card-body p-4">

                        <h1 class="text-center mb-4">
                            Sign Up
                        </h1>

                        <p class="text-center mb-4">
                            Please enter your information below.
                        </p>


                        <form id="signupForm">

                            <!-- Full Name -->
                            <div class="mb-3">
                                <label for="name" class="form-label">
                                    Full Name
                                </label>

                                <input 
                                    type="text" 
                                    class="form-control" 
                                    id="name"
                                    name="name"
                                    required
                                >
                            </div>


                            <!-- Age -->
                            <div class="mb-3">
                                <label for="age" class="form-label">
                                    Age
                                </label>

                                <input 
                                    type="number" 
                                    class="form-control" 
                                    id="age"
                                    name="age"
                                    min="1"
                                    required
                                >
                            </div>


                            <!-- Email -->
                            <div class="mb-3">
                                <label for="email" class="form-label">
                                    Email Address
                                </label>

                                <input 
                                    type="email" 
                                    class="form-control" 
                                    id="email"
                                    name="email"
                                    required
                                >
                            </div>


                            <!-- Phone -->
                            <div class="mb-3">
                                <label for="phone" class="form-label">
                                    Phone Number
                                    <span class="text-muted">(Optional)</span>
                                </label>

                                <input 
                                    type="tel" 
                                    class="form-control" 
                                    id="phone"
                                    name="phone"
                                >
                            </div>


                            <!-- Address -->
                            <div class="mb-3">
                                <label for="address" class="form-label">
                                    Address
                                </label>

                                <input 
                                    type="text" 
                                    class="form-control" 
                                    id="address"
                                    name="address"
                                    required
                                >
                            </div>


                            <!-- Submit -->
                            <div class="d-grid mt-4">

                                <button 
                                    type="submit" 
                                    class="btn btn-primary"
                                >
                                    Sign Up
                                </button>

                            </div>

                        </form>

                    </div>

                </div>

            </div>

        </div>

    </div>


    <!-- Bootstrap JavaScript -->
    <script 
        src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js">
    </script>

    <!-- Our Group JavaScript -->
    <script src="script.js"></script>

</body>
</html>
