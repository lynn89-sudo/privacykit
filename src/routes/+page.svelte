<script>
/*
    let privacyPolicy = [
        {
            "Identity Vault Verification": `Identity Vault will be used to verify your eligibility. No staff member outside HCB's operations team can directly access your data in the Identity Vault at <a href="auth.hackclub.com">auth.hackclub.com</a>. Cœur staff will only receive your full legal name, email, and eligibility to participate, outside information that we request from you on your submission form.`,
            "Authorized Access to Information": "All individuals that have access to your submission data and Identity Vault information are under NDA. This includes all staff for Cœur.",
            "Usage of Artificial Intelligence": "No PII (personally identifiable information), which includes emails, preferred names, legal names, and shipping addresses, will be given to any publically available AI model or platform. Statistics such as coding hours or heart balances may be given to a publically available AI model or platform.",
            "APIs": "No public API, behind auth or not, will contain PII (personally identifiable information), which includes emails, preferred names, legal names, and shipping addresses. All PII will be securely stored on Airtable, Fillout, or on a local computer.",
            "Date": "Feb 18, 2026"
        }
    ]
        */
    let privacyPolicy = [
        [
            {
            "title": "Identity Vault Verification",
            "message": `Identity Vault will be used to verify your eligibility. No staff member outside HCB's operations team can directly access your data in the Identity Vault at <a href="auth.hackclub.com">auth.hackclub.com</a>. Cœur staff will only receive your full legal name, email, and eligibility to participate, outside information that we request from you on your submission form.`
            },
            {
                "title": "Authorized Access to Information",
                "message": `All individuals that have access to your submission data and Identity Vault information are under NDA. This includes all staff for Cœur.`
            },
            {
                "title": "Usage of Artificial Intelligence",
                "message": `No PII (personally identifiable information), which includes emails, preferred names, legal names, and shipping addresses, will be given to any publically available AI model or platform. Statistics such as coding hours or heart balances may be given to a publically available AI model or platform.`
            },
            {
                "title": "APIs",
                "message": `No public API, behind auth or not, will contain PII (personally identifiable information), which includes emails, preferred names, legal names, and shipping addresses. All PII will be securely stored on Airtable, Fillout, or on a local computer.`
            }
        ]
    ]

    import Privacykit from "$lib/privacykit.svelte";
</script>

<h1>Welcome to your library project</h1>
<p>Create your package using @sveltejs/package and preview/showcase your work with SvelteKit</p>
<p>Visit <a href="https://svelte.dev/docs/kit">svelte.dev/docs/kit</a> to read the documentation</p>
<Privacykit policy={privacyPolicy}/>
