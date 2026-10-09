<Update label="October 9, 2026" tags={["Air"]}>

## New

### Appointment grouping
_Rolls out with next release · Front desk_

The appointments list can be grouped by facility, appointment type, or provider. Grouping by stage is available when check-in stages are turned on. Each group header shows how many appointments the group contains. Collapse a group to skip the appointments inside the group while moving through the list.

Where to find it: **Appointments**.

### Scheduled collections and revenue reports
_Beta customers · Billers_

Practices that already schedule reports can use **Add to schedule** on **Patient Collections**, **Custom Collections**, and **Encounter Revenue Activity**. The schedule stores the filters from the dialog, and the date range moves forward each time the report runs. On **Encounter Revenue Activity**, the as-of date cannot be chosen for a schedule. The dialog states: "As-of date will be set to the date of generation."

Where to find it: **My Reports** → open the report → **Add to schedule**.

### Patient discharge status
_Rolls out with next release · Providers and billers_

A discharged case can now carry a **Patient Discharge Status** (UB-04 Box 17) on the institutional claim. The select appears on an archived case and in the discharge dialog, and signing a discharge note shows the same select, prefilled from the case, and submits the status with the note. Leave the field blank and no status is sent, matching a discharge that has no status. A new case does not include the select.

### Units billed by CPT code
_Rolls out with next release · Billers_

**Financial Health Overview** adds a tile for billed units by CPT code, in **Leading indicators**, beside **Units per claim**. The chart shows the top five codes for the period, with a headline for total units and the change from the prior period, and the dates are always date of service, even when the dashboard is set to date posted. Hover a code to see the code's units and the code's share of every unit billed in the hovered bar, including codes outside the top five, and on a weekly bar the hover also shows how the code changed from the previous week. Facility, provider, payer, and assignee filters apply, and **View Claims** opens the claims behind the number.

Where to find it: **Dashboards** → **Financial Health Overview**.

### Final notice filter
_Rolls out with next release · Billers_

Bad Debt can filter charges by the latest final-notice attempt, and the only choices are **Sent** and **Failed**. The filter uses the most recent attempt, not an older notice on the same charge. A charge on the last step can sit in more than one place, and the step name alone does not separate a notice that went out from a notice that failed.

Where to find it: **Bad Debt**.

### Deposit insurance amount
_Rolls out with next release · Billers_

The deposit summary now lets you edit the insurance amount that was not posted through Athelas. The edit sidebar keeps a history of each edit.

Where to find it: **Remittances** → **Deposits** → open the deposit summary.

### Column order
_Rolls out with next release · Front desk, providers, and billers_

Drag a column header to rearrange the table. The order is saved in the browser where the header was dragged, and another computer keeps the default layout until a header is dragged on that computer. Selection columns, row actions, and other pinned columns stay in place. Reordering is available on the appointments inside a prior authorization, the **Prior Authorizations** list (**Pre-cert** and **Referral** remember separate orders), **Surgical History**, patient **Contacts**, and the patient-flow table on **Calendar**; the newer prior authorization table already keeps column order inside a saved view.

## Changed

### Appointments stage column
_Rolls out with next release · Front desk_

When patient flow is turned on for the Appointments worklist, the older **Stage** column is hidden and the **Visit Stage** filter is removed. Patient flow columns take the place of **Stage**. A saved view that still has **Stage** selected keeps the column hidden. The check-in tour skips the old Stage step. Practices without patient flow still see **Stage** and **Visit Stage**.

### Claim list place marker
_Rolls out with next release · Billers_

Returning to the claims list after working a claim used to land at a stale position when the claim no longer matched the filters, and the highlight had no row left to mark. If the claim is still in the list, the list scrolls to the row and highlights the row. If the claim has dropped out, a divider marks the old place: below the neighbor that sat above the missing row, or above the neighbor that sat below the missing row. When neither neighbor remains, the list scrolls as close as the remaining rows allow and shows no divider.

### Chart section counts
_Rolls out with next release · Providers_

A fixed section whose count is zero stays closed. Allergies and Attachments hide the caret, keep a header that cannot be opened, and leave the empty body closed. The panel still shows **No allergies.** when allergies are empty. A header with no count yet stays expandable and omits the number while the section is loading, after a load failure, or while a search still has more pages. Header counts sit on one line separated by a bar: the Allergies line looks like **2 Active | 1 Inactive**, and the Attachments line lists each source, for example **3 Patient | 0 Case | 0 Insurance Card | 5 Fax | 0 Chart Note**. Orders, Diagnosis, and Medications use that same line. Diagnosis keeps the same words as before. Medications keeps the existing wording, now separated with a bar. Past visit notes and Care Timeline are unchanged.

### Patient phone numbers
_Rolls out with next release · Front desk_

**Contact Information** on Demographics now shows **Home**, **Work**, and **Other** whenever a home, work, or other number is on file, and the primary number is labeled **Preferred phone**. A blank number stays hidden, so every saved number can be read without opening the editor.

Where to find it: **Demographics** → **Contact Information**.

### Pending check status
_Rolls out with next release · Billers_

**Posting Status** on the checks list included **Posted**, **Partially Posted**, and **Unposted**. The filter now also includes **Pending**, so you can find checks that need a manual review or checks that should be left unworked.

### Diagnosis visit dates
_Rolls out with next release · Providers_

**Visit date** on the Diagnosis filter now uses the same **After** and **Before** range as the attachments filter. The separate **Start date** and **End date** fields are gone. **Case**, **Provider**, and **Appointment type** stay on the filter.

### Health and wellness coach credential
_Rolls out with next release · Admins_

**Provider Credentials** now includes **NBC-HWC** (National Board Certified Health and Wellness Coach) under Nutrition and Dietetics, so you can assign **NBC-HWC** to a health coach.

Where to find it: **Preferences** → **Providers** → **Edit** → **Provider Credentials**.

## Fixed

- **New message** — **Messages** → **New message** now keeps a conversation to one patient and hides every other patient after the first selection, because adding several patients used to place every selected patient in one thread where each patient could read the others' messages; staff can still be selected together.
- **Import errors** — **Import** on **Import Errors** opens a new claim prefilled from the error, including patient, insurance, date of service, diagnosis codes, procedures, facility, and providers, instead of leaving **All Claims** open on an empty form.
- **Air Scribe** — A completed Air Scribe stays open when service selections are missing, and the services checkbox stays unchecked.
- **Intake forms** — A completed intake form that has a file now shows **Print** beside download; **Print** previously appeared only on a form that was not yet completed.
- **Prior authorization timeline** — Activity times now follow the practice time zone on the current timeline and the classic drawer, rather than one clock for every clinic; a short placeholder shows until the time zone loads, and a practice with no time zone on file uses the computer's time zone.
- **Scheduling conflicts** — The conflicts drawer lists openings and appointments by start time in the practice time zone, so an earlier opening appears before a later appointment.
- **Claim summary** — Returning from submission details keeps the claim panel scrolled to the same place.

</Update>
