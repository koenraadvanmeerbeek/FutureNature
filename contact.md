---
layout: page
title: Contact
permalink: /contact/
---
Feel free to reach out through the following channels:

<div class="contact-list">
  <div class="contact-item">
    <span class="icon-envelop contact-icon"></span>
    <a href="#" onclick="window.location='mailto:' + ['koenraad.vanmeerbeek', 'kuleuven.be'].join('@')">
      koenraad.vanmeerbeek@kuleuven.be
    </a>
  </div>

  <div class="contact-item">
    <span class="icon-bluesky contact-icon"></span>
    <a href="https://bsky.app/profile/kvanmeerbeek.bsky.social" target="_blank">
      @kvanmeerbeek.bsky.social
    </a>
  </div>

  <div class="contact-item">
    <span class="icon-linkedin2 contact-icon"></span>
    <a href="https://www.linkedin.com/in/koenraad-van-meerbeek-1b767b19/" target="_blank">
      LinkedIn Profile
    </a>
  </div>

  <div class="contact-item">
    <span class="icon-location contact-icon"></span>
    <a href="https://www.google.com/maps?q=Celestijnenlaan+200E,+3001+Leuven,+Belgium" target="_blank">
      Celestijnenlaan 200E, 3001 Leuven, Belgium
    </a>
  </div>
</div>

<style>
/* Container for the contact items */
.contact-list {
  display: flex;                /* Use flexbox for alignment */
  flex-wrap: wrap;              /* Wrap to the next line if items don't fit */
  gap: 1rem;                    /* Space between items */
  justify-content: space-between; /* Adjust spacing */
}

/* Individual contact items */
.contact-item {
  display: flex;                /* Align icon and text horizontally */
  align-items: center;          /* Vertically center icon and text */
  flex: 1 1 calc(50% - 1rem);   /* Make each item take up 50% of the width minus spacing */
  max-width: calc(50% - 1rem);  /* Ensure a maximum width of 50% */
  margin-bottom: 1rem;          /* Space between rows */
}

/* Icon styling */
.contact-icon {
  font-size: 24px;              /* Adjust icon size */
  margin-right: 0.5rem;         /* Space between icon and text */
  color: #006871ff;               /* Custom icon color */
}

/* Adjustments for smaller screens */
@media (max-width: 600px) {
  .contact-item {
    flex: 1 1 100%;             /* Make items stack vertically on small screens */
    max-width: 100%;            /* Full width for each item */
  }
}
</style>
