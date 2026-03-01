---
hero_title: "Get in Touch"
hero_subtitle: "Have a question, idea, or just want to say hello? I'd love to hear from you."
---

# Contact

Fill out the form below and I'll get back to you as soon as possible.

<div class="contact-form">
  <form
    action="https://formsubmit.co/your-email@example.com"
    method="POST"
    aria-label="Contact form"
    novalidate
  >
    <!-- Honeypot spam protection -->
    <input type="text" name="_honey" style="display:none" aria-hidden="true" tabindex="-1">
    <!-- Disable redirect after submit (FormSubmit default) -->
    <input type="hidden" name="_captcha" value="false">

    <div class="form-group">
      <label for="contact-name">Your Name <span aria-label="required">*</span></label>
      <input
        type="text"
        id="contact-name"
        name="name"
        placeholder="Jane Smith"
        required
        autocomplete="name"
        aria-required="true"
      >
    </div>

    <div class="form-group">
      <label for="contact-email">Email Address <span aria-label="required">*</span></label>
      <input
        type="email"
        id="contact-email"
        name="email"
        placeholder="jane@example.com"
        required
        autocomplete="email"
        aria-required="true"
      >
    </div>

    <div class="form-group">
      <label for="contact-subject">Subject</label>
      <input
        type="text"
        id="contact-subject"
        name="subject"
        placeholder="What's this about?"
        autocomplete="off"
      >
    </div>

    <div class="form-group">
      <label for="contact-message">Message <span aria-label="required">*</span></label>
      <textarea
        id="contact-message"
        name="message"
        placeholder="Write your message here…"
        required
        aria-required="true"
      ></textarea>
    </div>

    <button type="submit" class="form-submit">Send Message 📨</button>
  </form>
</div>

---

!!! tip "Form submissions"
    This form uses [FormSubmit](https://formsubmit.co/) for static-site form handling.
    Replace `your-email@example.com` in `contact.md` with your actual email address to start receiving messages.

---

## Other ways to reach me

| Method | Details |
|--------|---------|
| 🐙 GitHub | [github.com/YaelAvramovich](https://github.com/YaelAvramovich) |
