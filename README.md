
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title> 

    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet" href="form.css">

    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css"
          rel="stylesheet">

    <script src="script.js" defer></script>
</head>

<body>

    <!-- Navigation Bar -->
    <nav>
        <a href="index.html">Overview</a>
        <a href="signup.html">Attendees</a>
        <a href="events.html">Schedule</a>
        <a href="materials.html">Material Management</a>
    </nav>


    <!-- Main Content -->
    <section class="content container py-5" aria-label="Main content">

        <div class="text-center mb-4">
            <h1>Conference Registration</h1>
            <p class="text-muted">
                Enter your contact information and conference details below.
            </p>
        </div>

        <!-- Start Sign-Up Form -->
        <div class="registration-form mx-auto bg-white p-4 p-md-5 rounded shadow-sm">

            <form id="sign-up">

                <!-- Part 1: Point of Contact Information -->
                <fieldset class="mb-4">

                    <legend>Point of Contact</legend>

                    <div class="row">

                        <!-- First Name -->
                        <div class="form-item col-md-6 mb-3">
                            <label for="poc-firstname" class="form-label">
                                First Name
                            </label>
                            <input type="text"
                                   class="form-control"
                                   name="poc-firstname"
                                   id="poc-firstname"
                                   placeholder="Enter first name"
                                   required>
                        </div>

                        <!-- Last Name -->
                        <div class="form-item col-md-6 mb-3">
                            <label for="poc-lastname" class="form-label">
                                Last Name
                            </label>
                            <input type="text"
                                   class="form-control"
                                   name="poc-lastname"
                                   id="poc-lastname"
                                   placeholder="Enter last name"
                                   required>
                        </div>

                        <!-- Email -->
                        <div class="form-item col-md-6 mb-3">
                            <label for="poc-email" class="form-label">
                                Email Address
                            </label>
                            <input type="email"
                                   class="form-control"
                                   name="poc-email"
                                   id="poc-email"
                                   placeholder="example@email.com"
                                   required>
                        </div>

                        <!-- Phone -->
                        <div class="form-item col-md-6 mb-3">
                            <label for="poc-phone" class="form-label">
                                Phone Number
                            </label>
                            <input type="tel"
                                   class="form-control"
                                   name="poc-phone"
                                   id="poc-phone"
                                   placeholder="Optional">
                        </div>

                        <!-- Preferred Contact Method -->
                        <div class="form-item col-12 mb-3">

                            <label class="form-label d-block">
                                Preferred Method of Contact
                            </label>

                            <div class="form-check form-check-inline">
                                <input type="radio"
                                       class="form-check-input"
                                       name="poc-method"
                                       id="poc-method-email"
                                       value="email">
                                <label class="form-check-label"
                                       for="poc-method-email">
                                    Email
                                </label>
                            </div>

                            <div class="form-check form-check-inline">
                                <input type="radio"
                                       class="form-check-input"
                                       name="poc-method"
                                       id="poc-method-phone"
                                       value="phone">
                                <label class="form-check-label"
                                       for="poc-method-phone">
                                    Phone
                                </label>
                            </div>

                        </div>

                    </div>
                </fieldset>

                <!-- Part 2: Organization Information -->
                <fieldset class="mb-4">

                    <legend>Group Information</legend>

                    <div class="row">

                        <!-- Maximum Attendees -->
                        <div class="form-item col-md-6 mb-3">
                            <label for="max-attendees" class="form-label">
                                Maximum Number of Attendees
                            </label>

                            <select class="form-select"
                                    name="max-attendees"
                                    id="max-attendees">

                                <option value="250">250</option>
                                <option value="500">500</option>
                                <option value="1500">1,500</option>
                                <option value="2000">2,000</option>
                                <option value="2500">2,500</option>
                                <option value="3000">3,000</option>
                                <option value="4500">4,500</option>
                                <option value="5000">5,000</option>

                            </select>
                        </div>

                        <!-- Organization -->
                        <div class="form-item col-md-6 mb-3">
                            <label for="org-name" class="form-label">
                                Organization
                            </label>

                            <input type="text"
                                   class="form-control"
                                   name="org-name"
                                   id="org-name"
                                   placeholder="Enter organization name"
                                   required>
                        </div>

                        <!-- Industry -->
                        <div class="form-item col-md-6 mb-3">
                            <label for="org-industry" class="form-label">
                                Industry
                            </label>

                            <select class="form-select"
                                    name="org-industry"
                                    id="org-industry">

                                <option value="tech">Technology & Software</option>
                                <option value="heal">Healthcare & Life Sciences</option>
                                <option value="fina">Finance & Insurance</option>
                                <option value="educ">Education</option>
                                <option value="nonp">Non-Profit & Philanthropy</option>
                                <option value="gove">Government</option>
                                <option value="manu">Manufacturing & Logistics</option>
                                <option value="reta">Retail & Consumer Goods</option>
                                <option value="prof">Professional Services</option>
                                <option value="medi">Media & Entertainment</option>
                                <option value="ener">Energy & Utilities</option>
                                <option value="real">Real Estate & Construction</option>

                            </select>
                        </div>

                        <!-- Start Date -->
                        <div class="form-item col-md-6 mb-3">
                            <label for="org-date-start" class="form-label">
                                Requested Start Date
                            </label>

                            <input type="date"
                                   class="form-control"
                                   name="org-date-start"
                                   id="org-date-start">
                        </div>

                        <!-- End Date -->
                        <div class="form-item col-md-6 mb-3">
                            <label for="org-date-end" class="form-label">
                                Requested End Date
                            </label>

                            <input type="date"
                                   class="form-control"
                                   name="org-date-end"
                                   id="org-date-end">
                        </div>

                        <!-- Special Requests -->
                        <div class="form-item col-12 mb-3">
                            <label for="org-requests" class="form-label">
                                Special Requests
                            </label>

                            <textarea class="form-control"
                                      name="org-requests"
                                      id="org-requests"
                                      rows="4"
                                      placeholder="Enter any special requests here..."></textarea>
                        </div>

                    </div>
                </fieldset>

                <!-- Form Buttons -->
                <div class="d-flex flex-wrap gap-2">

                    <button type="submit" class="btn btn-primary">
                        Submit Registration
                    </button>

                    <button type= "reset" class="btn btn-outline-secondary">
                        Clear Form
                    </button>

                </div>

            </form>

        </div>

    </section>

</body>
</html>
