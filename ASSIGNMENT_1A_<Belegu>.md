# Assignment_1A


## Section 1: The Less-than-equal-4-Click User Journey Funnel

* **Starting State:** User lands on the DevPulse homepage and sees the core value proposition, landmark navigation links, and the "Deploy Free Cluster" CTA above the fold.

* **Action 1:** User clicks the navigation link to reach the cluster hosting tier/pricing section.

* **Action 2:** User compares and selects a cluster hosting tier from the Developer, Pro Cluster, and Enterprise Dedicated options.

* **Action 3:** User enters the required node count and log throughput into the workload estimation form.

* **Action 4:** User completes the required pre-registration fields and submits the form to request API sandbox provisioning details.

* **Terminal State:** User receives visual confirmation that the registration/provisioning request was successfully submitted.


## Section 2: The Don Norman Usability & Constraint Aidit

| Norman Principle               | UI Component / Feature                 | Context                                                                                | Specific HTML Element or Attribute Used to Enforce Principle |
| ------------------------------ | -------------------------------------- | -------------------------------------------------------------------------------------- | ------------------------------------------------------------ |
| **Signifier**                  | Primary Action Button (Above the fold) | Primary CTA for deploying a free cluster                                               | `<button>`                                                   |
| **Signifier**                  | Recommended Tier Indicator             | Identifies the Pro Cluster as the recommended/popular tier                             | `<mark>`                                                     |
| **Physical/System Constraint** | Workload Estimator: Node Count         | Restricts node count to valid numerical boundaries without JavaScript                  | `<input type="number" min="..." max="..." step="...">`       |
| **Physical/System Constraint** | Operator Contact Field                 | Prevents the required contact field from being left blank when the form is submitted   | `<input type="email" required>`                              |
| **Feedback Loop**              | Form Submission / Live Anchors         | Confirms that the form was submitted                                                   | `<form>`                                                     |


## Section 3: Semantic Component & Layout Tree


***
   

* `html`

  * `head`

    * `title` — DevPulse
  * `body`

    * `header`

      * `nav`

        * `a` — Navigation link
        * `a` — Navigation link
        * `a` — Navigation link
        * `button` — Deploy Free Cluster
    * `main`

      * `section` — DevPulse Introduction

        * `h1` — DevPulse
        * `p` — Core value proposition
      * `section` — Infrastructure Features

        * `h2` — Infrastructure Features
        * `article`

          * `h3` — Latency Tracking
          * `p` — Feature description
        * `article`

          * `h3` — Log Aggregation
          * `p` — Feature description
        * `article`

          * `h3` — Auto-Remediation
          * `p` — Feature description
      * `section` — Cluster Hosting Tiers

        * `h2` — Cluster Hosting Tiers
        * `article`

          * `h3` — Developer
          * `p` — Tier description
        * `article`

          * `h3` — Pro Cluster
          * `mark` — Most Popular
          * `p` — Tier description
        * `article`

          * `h3` — Enterprise Dedicated
          * `p` — Tier description
      * `section` — Workload Estimator

        * `h2` — Workload Estimator
        * `form`

          * `label` — Node Count
          * `input`

            * `type="number"`
            * `min="..."`
            * `max="..."`
            * `step="..."`
          * `label` — Log Throughput
          * `input`

            * `type="number"`
            * `min="..."`
            * `max="..."`
            * `step="..."`
      * `section` — API Sandbox Registration

        * `h2` — API Sandbox Registration
        * `form`

          * `label` — Email
          * `input`

            * `type="email"`
            * `required`
          * `button`

            * `type="submit"`
    * `footer`
***

## Section 4: Evaluation Rubric 

| Evaluation Dimension                                     | Points | Full Points                                                                                                             | Partial Credit (10-30% penalty)                                                                              | Unsatisfactory (Flat 30% or more penalty)                          |
| -------------------------------------------------------- | ------ | ----------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------ | 
| **User Journey Funnel (Section 1)**                      | 6      | Deconstructs user conversion into <=4 discrete, logical steps mapping directly to the 5 user stories.                   | Exceeds 4 interactions or omits critical steps (e.g., jumps straight to submission without selecting tiers). | Incoherent or missing interaction flow.                            |
| **Norman UX & Constraint Audit**                         | 8      | Accurately identifies signifiers, constraints, and feedback states using native HTML tags and attributes.               | Misidentifies Norman principles or relies on generic non-semantic elements.                                  | Incomplete audit table; failure to explain constraint enforcement. |
| **Semantic Hierarchy & Landmark Discipline (Section 3)** | 10     | Tree addresses all content requirements and demonstrates strict semantic nesting with correct heading order.            | Overuses generic <div> tags for landmark sections or skips heading levels.                                   | Monolithic <div> structure; non-semantic layout.                   |
|**Form Constraint Modeling (Section 3)**                  | 6      | Form inputs explicitly annotate attributes (required, type="email", min, max, step) preventing illegal states natively. | Form inputs lack explicit boundary attributes or rely on assumed JavaScript handling.                        |Form tags are unannotated; missing labels or input types.           |
