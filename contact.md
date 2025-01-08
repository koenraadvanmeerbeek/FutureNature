---
layout: page
title: Contact
permalink: /contact/
---
Feel free to reach out through the following channels:

<div class="contact-list">
  <div class="contact-item">
    <a href="#" onclick="window.location='mailto:' + ['koenraad.vanmeerbeek', 'kuleuven.be'].join('@')" class="contact-link">
      <span class="icon-envelop contact-icon"></span>
      <span class="contact-text">koenraad.vanmeerbeek[at]kuleuven.be</span>
    </a>
  </div>

  <div class="contact-item">
    <a href="https://bsky.app/profile/kvanmeerbeek.bsky.social" target="_blank" class="contact-link">
      <span class="icon-bluesky contact-icon"></span>
      <span class="contact-text">Follow me on Bluesky</span>
    </a>
  </div>

  <div class="contact-item">
    <a href="https://www.linkedin.com/in/koenraad-van-meerbeek-1b767b19/" target="_blank" class="contact-link">
      <span class="icon-linkedin2 contact-icon"></span>
      <span class="contact-text">Follow me on LinkedIn</span>
    </a>
  </div>

  <div class="contact-item">
    <a href="https://www.google.com/maps?q=Celestijnenlaan+200E,+3001+Leuven,+Belgium" target="_blank" class="contact-link">
      <span class="icon-location contact-icon"></span>
      <span class="contact-text">Celestijnenlaan 200E, 3001 Leuven, Belgium</span>
    </a>
  </div>
</div>

<style>
/* General container for the contact list */
.contact-list {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(150px, 1fr)); /* Adjust column minimum to 150px for more flexibility */
  gap: 1rem; /* Space between items */
  justify-items: center; /* Centers items within the grid */
  width: 100%; /* Ensure the grid container takes the full width */
  max-width: 1200px; /* Optional: Restrict maximum width for better design on large screens */
  margin: 0 auto; /* Center the grid container horizontally */
}

/* Individual contact item */
.contact-item {
  text-align: center; /* Center align icon and text */
}

/* Contact link to include both icon and text */
.contact-link {
  display: flex;
  flex-direction: column; /* Stack icon and text */
  align-items: center; /* Center content */
  text-decoration: none; /* Remove underline */
  color: inherit; /* Use inherited color */
  transition: transform 0.2s ease-in-out, color 0.2s ease-in-out; /* Add hover effect */
}

/* Icon styles */
.contact-icon {
  font-size: 40px; /* Size of the icon */
  margin-bottom: 0.5rem; /* Space between icon and text */
  color: #006871ff; /* Icon color */
  transition: transform 0.2s ease-in-out, color 0.2s ease-in-out; /* Hover effect */
}

/* Text styles */
.contact-text {
  font-size: 16px;
  color: #333; /* Default text color */
  transition: color 0.2s ease-in-out; /* Hover effect */
}

/* Hover effect */
.contact-link:hover .contact-icon {
  transform: scale(1.1); /* Slightly enlarge the icon */
  color: #a4d5d9ff; /* Change color on hover */
}

.contact-link:hover .contact-text {
  color: #a4d5d9ff; /* Change text color on hover */
}

</style>
