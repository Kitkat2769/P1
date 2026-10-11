
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Conference Registration</title>

    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet" href="form.css">

    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css"
          rel="stylesheet">

    <script src="script.js" defer></script>
</head>

<body>

    <nav>
        <a href="index.html">Overview</a>
        <a href="signup.html" aria-current="page">Attendees</a>
        <a href="events.html">Schedule</a>
        <a href="materials.html">Material Management</a>
    </nav>

    <section class="banner" aria-label="Page banner">
        <img src="imgs/Banner.jpg" alt="Conference banner">
    </section>

    <main class="container py-5">

        <header class="text-center mb-4">
            <h1>Conference Registration</h1>
            <p>Register your organization and manage conference requests.</p>
        </header>

        <section class="card shadow-sm registration-card">
            <div class="card-body p-4">

                <div id="status-message"
                     class="alert d-none"
                     role="status"
                     aria-live="polite"></div>

                <form id="sign-up" novalidate>

                    <input type="hidden" id="registration-id">

                    <fieldset class="mb-4">
                        <legend>Point of Contact</legend>

                        <div class="row g-3">

                            <div class="col-md-6 form-item">
                                <label for="poc-firstname" class="form-label">
                                    First Name *
                                </label>
                                <input type="text"
                                       class="form-control"
                                       name="poc-firstname"
                                       id="poc-firstname"
                                       required>
                                <div class="invalid-feedback">
                                    Enter a first name.
                                </div>
                            </div>

                            <div class="col-md-6 form-item">
                                <label for="poc-lastname" class="form-label">
                                    Last Name *
                                </label>
                                <input type="text"
                                       class="form-control"
                                       name="poc-lastname"
                                       id="poc-lastname"
                                       required>
                                <div class="invalid-feedback">
                                    Enter a last name.
                                </div>
                            </div>

                            <div class="col-md-6 form-item">
                                <label for="poc-email" class="form-label">
                                    Email Address *
                                </label>
                                <input type="email"
                                       class="form-control"
                                       name="poc-email"
                                       id="poc-email"
                                       required>
                                <div class="invalid-feedback">
                                    Enter a valid email address.
                                </div>
                            </div>

                            <div class="col-md-6 form-item">
                                <label for="poc-phone" class="form-label">
                                    Phone Number
                                </label>
                                <input type="tel"
                                       class="form-control"
                                       name="poc-phone"
                                       id="poc-phone"
                                       placeholder="Optional">
                                <div class="invalid-feedback">
                                    Enter a valid phone number.
                                </div>
                            </div>

                            <div class="col-12 form-item">
                                <label class="form-label d-block">
                                    Preferred Method of Contact
                                </label>

                                <div class="form-check form-check-inline">
                                    <input type="radio"
                                           class="form-check-input"
                                           name="poc-method"
                                           id="poc-method-email"
                                           value="Email">
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
                                           value="Phone">
                                    <label class="form-check-label"
                                           for="poc-method-phone">
                                        Phone
                                    </label>
                                </div>
                            </div>

                        </div>
                    </fieldset>

                    <fieldset class="mb-4">
                        <legend>Group Information</legend>

                        <div class="row g-3">

                            <div class="col-md-6 form-item">
                                <label for="max-attendees" class="form-label">
                                    Maximum Number of Attendees
                                </label>
                                <select class="form-select"
                                        name="max-attendees"
                                        id="max-attendees"
                                        required>
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

                            <div class="col-md-6 form-item">
                                <label for="org-name" class="form-label">
                                    Organization *
                                </label>
                                <input type="text"
                                       class="form-control"
                                       name="org-name"
                                       id="org-name"
                                       required>
                                <div class="invalid-feedback">
                                    Enter an organization name.
                                </div>
                            </div>

                            <div class="col-md-6 form-item">
                                <label for="org-industry" class="form-label">
                                    Industry
                                </label>
                                <select class="form-select"
                                        name="org-industry"
                                        id="org-industry">
                                    <option value="Technology & Software">Technology & Software</option>
                                    <option value="Healthcare & Life Sciences">Healthcare & Life Sciences</option>
                                    <option value="Finance & Insurance">Finance & Insurance</option>
                                    <option value="Education">Education</option>
                                    <option value="Non-Profit & Philanthropy">Non-Profit & Philanthropy</option>
                                    <option value="Government">Government</option>
                                    <option value="Manufacturing & Logistics">Manufacturing & Logistics</option>
                                    <option value="Retail & Consumer Goods">Retail & Consumer Goods</option>
                                    <option value="Professional Services">Professional Services</option>
                                    <option value="Media & Entertainment">Media & Entertainment</option>
                                    <option value="Energy & Utilities">Energy & Utilities</option>
                                    <option value="Real Estate & Construction">Real Estate & Construction</option>
                                </select>
                            </div>

                            <div class="col-md-6 form-item">
                                <label for="org-date-start" class="form-label">
                                    Requested Start Date
                                </label>
                                <input type="date"
                                       class="form-control"
                                       name="org-date-start"
                                       id="org-date-start">
                            </div>

                            <div class="col-md-6 form-item">
                                <label for="org-date-end" class="form-label">
                                    Requested End Date
                                </label>
                                <input type="date"
                                       class="form-control"
                                       name="org-date-end"
                                       id="org-date-end">
                            </div>

                            <div class="col-12 form-item">
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

                    <div class="d-flex flex-wrap gap-2">
                        <button type="submit"
                                id="submit-button"
                                class="btn btn-primary">
                            Submit Registration
                        </button>

                        <button type="button"
                                id="cancel-edit"
                                class="btn btn-outline-secondary d-none">
                            Cancel Edit
                        </button>

                        <button type="reset"
                                id="clear-form"
                                class="btn btn-outline-secondary">
                            Clear Form
                        </button>
                    </div>

                    <p class="text-muted small mt-3">
                        * Required fields
                    </p>

                </form>
            </div>
        </section>

        <section class="mt-5" aria-labelledby="registrations-heading">

            <div class="d-flex justify-content-between align-items-center
                        flex-wrap gap-2 mb-3">
                <div>
                    <h2 id="registrations-heading">Conference Registrations</h2>
                    <p class="text-muted mb-0">
                        Total registrations:
                        <strong id="registration-count">0</strong>
                    </p>
                </div>

                <button type="button"
                        id="export-json"
                        class="btn btn-outline-primary">
                    Download JSON
                </button>
            </div>

            <div class="table-responsive">
                <table class="table table-striped table-hover align-middle">
                    <thead class="table-dark">
                        <tr>
                            <th>Contact</th>
                            <th>Email</th>
                            <th>Organization</th>
                            <th>Capacity</th>
                            <th>Start Date</th>
                            <th>End Date</th>
                            <th>Actions</th>
                        </tr>
                    </thead>

                    <tbody id="registration-table-body">
                        <tr>
                            <td colspan="7" class="text-center">
                                No registrations yet.
                            </td>
                        </tr>
                    </tbody>
                </table>
            </div>

        </section>

    </main>

    <footer class="text-center py-4 mt-5 border-top">
        <p>&copy; 2026 Conference Event Organizer. All rights reserved.</p>
    </footer>

</body>
</html>
