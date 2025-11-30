<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>001 Agency — Build Your Brand</title>
  <meta name="description" content="001 Agency — Branding, Websites & Automation | Ultra Clean One-Page Funnel" />
  <style>
    :root{
      --blue:#0A66C2; --deep:#073A73; --soft:#7AB9FF; --white:#ffffff; --dark:#1A1A1A;
      --maxw:980px;
    }
    *{box-sizing:border-box}
    body{font-family:Inter, system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial; color:var(--dark); margin:0; background:#f7fbff}
    .wrap{max-width:var(--maxw); margin:40px auto; padding:28px}
    header{display:flex;align-items:center;justify-content:space-between}
    .brand{display:flex;gap:14px;align-items:center}
    .logo-circle{width:56px;height:56px;border-radius:8px;background:linear-gradient(135deg,var(--blue),var(--soft));display:flex;align-items:center;justify-content:center;color:#fff;font-weight:700;font-family:Montserrat, sans-serif}
    h1{font-family:Montserrat, sans-serif;margin:0;font-size:28px}
    p.lead{margin:6px 0 0;color:#334155}
    .hero{display:grid;grid-template-columns:1fr 360px;gap:28px;margin-top:30px}
    .card{background:#fff;border-radius:12px;padding:20px;box-shadow:0 6px 18px rgba(10,66,194,0.06)}
    .cta-group{display:flex;flex-direction:column;gap:12px}
    .btn{display:inline-flex;align-items:center;gap:10px;padding:12px 16px;border-radius:8px;border:0;cursor:pointer;font-weight:600}
    .btn-blue{background:var(--blue);color:#fff}
    .btn-outline{background:transparent;border:1px solid rgba(10,102,194,0.12);color:var(--deep)}
    .packages{display:flex;gap:14px;margin-top:22px}
    .pkg{flex:1;padding:18px;border-radius:10px;background:linear-gradient(180deg,#fff,#f8fdff);border:1px solid rgba(10,66,194,0.04)}
    .pkg h3{margin:6px 0}
    .steps{display:flex;gap:10px;margin-top:18px}
    .step{flex:1;background:linear-gradient(180deg,#fff,#f7fbff);padding:14px;border-radius:10px;border:1px solid rgba(10,66,194,0.04)}
    footer{margin-top:30px;text-align:center;color:#64748b; font-size:13px}
    .center{text-align:center}
    .badge{display:inline-block;padding:8px 12px;background:rgba(10,102,194,0.08);color:var(--deep);border-radius:999px;font-weight:600}
    /* modal */
    .modal{position:fixed;inset:0;display:none;align-items:center;justify-content:center;background:rgba(2,6,23,0.4);}
    .modal.show{display:flex}
    .modal-card{width:420px;background:#fff;padding:20px;border-radius:12px}
    .form-row{margin:10px 0}
    input,textarea,select{width:100%;padding:10px;border-radius:8px;border:1px solid #e6eef9;font-size:14px}
    .small{font-size:13px;color:#475569}
    @media(max-width:880px){.hero{grid-template-columns:1fr;padding:0}.packages{flex-direction:column}.hero{grid-template-columns:1fr}}
  </style>
</head>
<body>
  <div class="wrap">
    <header>
      <div class="brand">
        <div class="logo-circle">001</div>
        <div>
          <h1>001 Agency</h1>
          <div class="small">Corporate Branding • Websites • Automation</div>
        </div>
      </div>
      <div class="badge">Ultra Clean Funnel</div>
    </header>

    <section class="hero">
      <div>
        <div class="card">
          <h2>Build Your Brand. Launch Your Website. Automate Your Business.</h2>
          <p class="lead">Fast corporate-grade branding, websites and WhatsApp automation. Choose a package below and start now — payment triggers onboarding automatically.</p>

          <div class="packages">
            <div class="pkg">
              <h3>Starter</h3>
              <div class="small">29,999 KES</div>
              <ul>
                <li>Logo (3 concepts)</li>
                <li>Social + WhatsApp setup</li>
                <li>3 templates</li>
                <li>7-day support</li>
              </ul>
              <button class="btn btn-outline" onclick="startPackage('Starter','29999')">Get Starter</button>
            </div>
            <div class="pkg">
              <h3>Business</h3>
              <div class="small">59,999 KES — Most Popular</div>
              <ul>
                <li>Everything in Starter</li>
                <li>5-page website</li>
                <li>WhatsApp automation</li>
                <li>30-day support</li>
              </ul>
              <button class="btn btn-blue" onclick="startPackage('Business','59999')">Get Business</button>
            </div>
            <div class="pkg">
              <h3>Premium</h3>
              <div class="small">99,999 KES</div>
              <ul>
                <li>Premium branding</li>
                <li>Full website + integrations</li>
                <li>Priority support</li>
              </ul>
              <button class="btn btn-outline" onclick="startPackage('Premium','99999')">Get Premium</button>
            </div>
          </div>

          <div class="steps">
            <div class="step center">
              <strong>Step 1</strong>
              <div class="small">Choose package</div>
            </div>
            <div class="step center">
              <strong>Step 2</strong>
              <div class="small">Pay (M-Pesa / Paybill)</div>
            </div>
            <div class="step center">
              <strong>Step 3</strong>
              <div class="small">Fill onboarding form</div>
            </div>
          </div>

        </div>

        <div style="margin-top:18px;text-align:center">
          <button class="btn btn-blue" onclick="openWhatsApp()">Chat on WhatsApp</button>
          <button class="btn btn-outline" onclick="openModal()">Pay with Paybill</button>
        </div>

      </div>

      <aside>
        <div class="card">
          <h3 class="center">Why 001 Agency</h3>
          <ul>
            <li>Corporate designs trusted by businesses</li>
            <li>Automation that frees your time</li>
            <li>Fast delivery: 72 hours — 7 days</li>
            <li>Payment-first onboarding</li>
          </ul>
          <div style="margin-top:10px">
            <strong>Contact</strong>
            <div class="small">Nairobi, Kenya • 001 Agency</div>
            <div style="margin-top:8px">
              <button class="btn btn-blue" onclick="openWhatsApp()">Message</button>
            </div>
          </div>
        </div>

        <div class="card" style="margin-top:12px">
          <h4 class="center">Quick FAQ</h4>
          <div class="small">Delivery time: 72 hrs - 7 days. Payment triggers onboarding. Support included per package.</div>
        </div>
      </aside>
    </section>

    <footer>
      001 Agency — Corporate Branding, Websites & Automation • © 2025
    </footer>
  </div>

  <!-- Payment modal + onboarding -->
  <div id="modal" class="modal">
    <div class="modal-card">
      <h3>Pay with M-Pesa Paybill</h3>
      <p class="small">Use Paybill: <strong id="paybill-number">[PAYBILL_NUMBER]</strong> • Account: <strong id="acc-ref">001AGENCY</strong></p>
      <div class="form-row">
        <label class="small">Selected Package</label>
        <input id="pkg" disabled />
      </div>
      <div class="form-row">
        <label class="small">Amount (KES)</label>
        <input id="amount" disabled />
      </div>
      <div class="form-row">
        <label class="small">Your Business / Name</label>
        <input id="client-name" placeholder="e.g. Prime Logistics" />
      </div>
      <div class="form-row">
        <label class="small">Phone (07...)</label>
        <input id="client-phone" placeholder="2547xxxxxxxx" />
      </div>
      <div style="display:flex;gap:8px;margin-top:10px">
        <button class="btn btn-blue" onclick="confirmOnPayment()">I will pay now (I used Paybill)</button>
        <button class="btn btn-outline" onclick="closeModal()">Cancel</button>
      </div>
      <p class="small" style="margin-top:8px">After you confirm, our system will ask for the M-Pesa transaction code and automatically trigger onboarding.</p>
    </div>
  </div>

  <script>
    // --- CONFIGURE THESE BEFORE DEPLOY ---
    const CONFIG = {
      PAYBILL: '123456',              // <<< replace with your Paybill number
      PAYBILL_ACCOUNT: '001AGENCY',
      WEBHOOK_URL: 'https://hook.example.com/001agency', // <<< replace with your Make.com / Zapier webhook
      WHATSAPP_NUMBER: '254700000000' // <<< business number for wa.me links (country code, no plus)
    }

    document.getElementById('paybill-number').textContent = CONFIG.PAYBILL;

    function startPackage(name, amount){
      document.getElementById('pkg').value = name;
      document.getElementById('amount').value = amount;
      openModal();
    }

    function openModal(){document.getElementById('modal').classList.add('show')}
    function closeModal(){document.getElementById('modal').classList.remove('show')}

    function openWhatsApp(){
      const msg = encodeURIComponent('Hello 001 Agency — I want details about packages and onboarding.');
      window.open('https://wa.me/' + CONFIG.WHATSAPP_NUMBER + '?text=' + msg, '_blank');
    }

    function confirmOnPayment(){
      const name = document.getElementById('client-name').value || 'Client';
      const phone = document.getElementById('client-phone').value || '';
      const pkg = document.getElementById('pkg').value;
      const amount = document.getElementById('amount').value;
      if(!phone){alert('Please add your phone number to continue.');return}

      // Push lead to webhook for automation engine (Make.com / Zapier)
      const payload = {package:pkg,amount:amount,client_name:name,phone:phone,paybill:CONFIG.PAYBILL,account:CONFIG.PAYBILL_ACCOUNT,timestamp:new Date().toISOString()};

      fetch(CONFIG.WEBHOOK_URL,{
        method:'POST',headers:{'Content-Type':'application/json'},body:JSON.stringify(payload)
      }).then(r=>{
        if(r.ok){
          alert('Thanks — we received your confirmation. Please pay via M-Pesa Paybill now.\nAfter payment, reply with the M-Pesa code to our WhatsApp or use the confirmation link.')
          closeModal();
          // Optionally open WhatsApp with a prefilled message to paste transaction code
          const waMsg = encodeURIComponent('I have paid ' + amount + ' KES for ' + pkg + '. M-Pesa code: [TYPE CODE HERE]');
          window.open('https://wa.me/' + CONFIG.WHATSAPP_NUMBER + '?text=' + waMsg, '_blank');
        } else {alert('Could not confirm now. Please try messaging us on WhatsApp.')}
      }).catch(e=>{alert('Network error — please message us on WhatsApp.');console.error(e)})
    }
  </script>

  <!--
    ADDITIONAL DEPLOY NOTES (DO NOT REMOVE):

    1) Replace CONFIG.PAYBILL with your M-Pesa Paybill number.
    2) Replace CONFIG.WEBHOOK_URL with your Make.com / Zapier webhook URL.
    3) Replace CONFIG.WHATSAPP_NUMBER with your WhatsApp Business-enabled number (country code, no +).

    AUTOMATION (Make.com / Zapier) SUGGESTED FLOW:
    - Trigger: Webhook receives payload from this page (package,amount,name,phone,timestamp)
    - Action 1: Create row in Google Sheets (lead tracker)
    - Action 2: Create task in Notion/Trello (project board) with package details
    - Action 3: Send WhatsApp message via WhatsApp Business API provider (360dialog/Twilio) with onboarding form link
    - Action 4: When payment confirmed (MPESA confirmation via MPESA API or manual check), update sheet and change task status to 'In Progress'
    - Action 5: Create folder in Google Drive and notify freelancer Slack/Email

    WHATSAPP BOT SCRIPT (for automation):
    - Auto-Greet: "Welcome to 001 Agency 👋 We build branding, websites & automation. Reply 1 for Packages, 2 to Book, 3 to Pay."
    - If '1' -> send packages PDF and short CTAs
    - If '2' -> ask: Business name? Service needed? Budget? Start date?
    - If '3' -> send paybill details and request transaction code
    - On receiving transaction code -> validate (MPESA API or manual) -> if valid send onboarding form link and create project

    SAMPLE ONBOARDING FORM FIELDS:
    - Business Name
    - Primary Contact
    - Phone
    - Email
    - Short description of business
    - Logo files (if any)
    - Preferred colors / notes

    MPESA INTEGRATION NOTES:
    - For instant verification you can integrate Safaricom's Daraja APIs or use a payments provider (Paystack, Flutterwave) that supports MPesa.
    - If using Daraja, set up webhook for STK Push or Lipa Na MPesa responses to your server, then forward confirmation to Make.com / Zapier.

  -->
</body>
</html>
# 001STUNNA
BEST 001
