<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Your GoToGo Ticket</title>
  <link rel="shortcut icon" href="assets/GoToGo Final Logos/GoToGo Final Logos/G2G Fleet - Inverse Black.png" type="image/x-icon">
  <script src="https://cdnjs.cloudflare.com/ajax/libs/html2pdf.js/0.10.1/html2pdf.bundle.min.js"></script>
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600;700&display=swap" rel="stylesheet">
  <style>
    body {
      font-family: 'Montserrat', sans-serif;
      margin: 0;
      background: #f5f5f5;
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;
      min-height: 100vh;
    }

    .ticket-scale-wrapper {
      width: 375px;
      height: 667px;
      transform-origin: top left;
    }

    .ticket-wrapper {
      width: 375px;
      height: 667px;
      background: white;
      padding: 20px;
      box-sizing: border-box;
      border: 1px solid #ccc;
      border-radius: 10px;
      box-shadow: 0 0 15px rgba(0, 0, 0, 0.1);
      overflow: hidden;
    }

    .download-btn {
      margin-top: 20px;
      background: #f1c40f;
      border: none;
      padding: 12px 30px;
      font-size: 16px;
      font-weight: bold;
      border-radius: 6px;
      cursor: pointer;
      transition: 0.3s ease;
    }

    .download-btn:hover {
      background: #d4ac0d;
    }

    /* Responsive scaling for small viewports */
    @media (max-width: 400px) {
      .ticket-scale-wrapper {
        transform: scale(0.9);
      }
    }

    @media (max-width: 360px) {
      .ticket-scale-wrapper {
        transform: scale(0.8);
      }
    }

    @media (max-width: 320px) {
      .ticket-scale-wrapper {
        transform: scale(0.75);
      }
    }
  </style>
</head>
<body>
<div style="width: 100%;">
  <img src="./assets/airport-bg.png" alt="" width="100%" style=" position: fixed; z-index: -1;">
</div>

  <h3>Download Your Ticket</h3>

  <!-- Fixed-scale container -->
  <div class="ticket-scale-wrapper" id="ticket">
    <div class="ticket-wrapper">
      <!-- Header -->
      <div style="display: flex; justify-content: space-around; align-items: center; background: #eebd36; padding: 0px; gap: 20px;">
        <img src="./assets/logo.jpg" alt="GoToGo Logo" style="height: 40px; padding: 4px;">
        <div style="font-weight: bold; font-size: 12px;">SHUTTLE TO AIRPORT</div>
      </div>

      <div style="margin-top: 10px; display: flex; justify-content: space-between; ">
        <div>
        <div style="color: #737373; font-size: 12px; font-weight: bold;">NAME OF PASSENGER</div>
        <div style="font-weight: bold; color: #004aad; font-size: 12px;">JOHNEY LIVER D’CRUIZE</div>
        </div>
        <div style="display: flex; align-items: center;">
          <div style="color: #737373; font-size: 12px; font-weight: bold;">TICKET #</div>
          <div style="border: 2px solid #000; border-radius: 18px; padding: 5px 8px; font-weight: bold; color: #004aad; font-size: 12px;">G2G-AS-SH-001</div>
        </div>
      </div>

      <div style="margin-top: 10px; display: flex; justify-content: space-between;">
        <div>
        <div style="color: #737373; font-size: 12px; font-weight: bold;">SHUTTLE BOARDING TIME</div>
        <div style="display: flex; gap: 10px; margin-top: 5px; color: #004aad;">
          <div style="font-weight: bold; text-align: center; border-radius: 50%; border: 2px solid #000; width: 30px; height: 30px; display: flex; flex-direction: column; justify-content: center; align-items: center; padding: 2px; font-size: 12px;">
            6<br><span style="font-size: 10px; font-weight: bold;">Am</span>
          </div>
          <div style="font-weight: bold; text-align: center; border-radius: 50%; border: 2px solid #000; width: 30px; height: 30px; display: flex; flex-direction: column; justify-content: center; align-items: center; padding: 2px; font-size: 12px;">
            7<br><span style="font-size: 10px; font-weight: bold;">Am</span>
          </div>
          <div style="font-weight: bold; text-align: center; border-radius: 50%; border: 2px solid #000; width: 30px; height: 30px; display: flex; flex-direction: column; justify-content: center; align-items: center; padding: 2px; font-size: 12px;">
            8<br><span style="font-size: 10px; font-weight: bold;">Am</span>
          </div>
        </div>
        </div>
        <div>
          <div style="color: #737373; font-size: 12px; font-weight: bold;">DROP TERMINAL</div>
          <div style="display: flex; gap: 5px; margin-top: 5px; color: #004aad;">
            <div style=" font-weight: bold; text-align: center; border-radius: 50%; border: 2px solid #000; width: 30px; height: 30px; display: flex; flex-direction: column; justify-content: center; align-items: center; padding: 2px; font-size: 12px;">
            T1
          </div>
          <div style=" font-weight: bold; text-align: center; border-radius: 50%; border: 2px solid #000; width: 30px; height: 30px; display: flex; flex-direction: column; justify-content: center; align-items: center; padding: 2px; font-size: 12px;">
            T2
          </div>
          <div style=" font-weight: bold; text-align: center; border-radius: 50%; border: 2px solid #000; width: 30px; height: 30px; display: flex; flex-direction: column; justify-content: center; align-items: center; padding: 2px; font-size: 12px;">
            T3
          </div>
          </div>
        </div>
      </div>

      <div style="margin-top: 10px; display: flex; justify-content: space-between; font-size: 12px;">
        <div>
          <div style="color: #737373; font-weight: bold;">PICKUP DATE</div>
          <div style="font-weight: bold; color: #004aad;">MAY 01</div>
        </div>
        <div>
          <div style="color: #737373; font-weight: bold;">PICKUP LOCATION</div>
        <div style="font-weight: bold; color: #004aad;">SUNDAY HOTEL</div>
        </div>
        
      </div>

      <div style="margin-top: 10px; display: flex; justify-content: space-between; font-size: 12px;">

        <div>
          <div style="color: #737373;font-weight: bold;">PAYMENT STATUS</div>
          <div style="font-weight: bold; color: #004aad;">PAID</div>
        </div>
        <div>
        <div style="color: #737373;font-weight: bold;">PICKUP ADDRESS</div>
        <div style="font-weight: bold; color: #004aad;">Sec 66, GGN</div>
        </div>
        
      </div>


      <div style="border: 3px solid #eebd36; padding: 10px; margin-top: 10px; border-radius: 19px;">
        <div style="font-weight: bold; font-size: 12px; background: #eebd36; width: 230px; border-radius: 8px; padding: 2px; position: relative; top: -20px; left: 50px;">Travel Assistance: (+91) 7065 650 650</div>
        <div style="font-size: 8px;  text-align: justify; margin-top: -10px;" >
          For <span style="font-weight: bold; color: #737373;">International Travel,</span> please arrive 4 hours before the flight.
For <span style="font-weight: bold; color: #737373;">Domestic Travel,</span> please arrive 3 hours before the flight. 
Please take care of your belongings while on board.
        </div>
      </div>

      <div style="margin-top: 10px;">
        <h4 style="margin-bottom: 5px; font-size: 12px;">TERMS & CONDITIONS</h4>
        <ul style="font-size: 8px; padding-left: 20px; text-align: justify;">
  <li><strong>Seating Policy:</strong> Seats are not pre-assigned. Seating is strictly on a first-come, first-served basis.</li>
  <li><strong>Departure Timings:</strong> The shuttle will depart strictly as per the scheduled time. There will be no additional waiting. Passengers are requested to arrive at the pickup point well in advance to avoid missing the shuttle.</li>
  <li><strong>No-Show Policy:</strong> In case of a no-show, the booking will be considered fully charged and non-refundable.</li>
  <li><strong>Cancellation & Transfer:</strong> This ticket is non-cancellable, non-transferable, and non-refundable under normal circumstances.</li>
  <li><strong>Exceptions (Force Majeure):</strong> In the event of unforeseen conditions (e.g., natural disasters, strikes, etc.) affecting service operations, alternate arrangements or refunds will be offered based on the situation and feasibility.</li>
  <li><strong>Refund Processing:</strong> If a refund is applicable, it will be processed within 14 working days.</li>
  <li><strong>Service Disclaimer:</strong> GoToGo shall not be held responsible for flight delays, traffic disruptions, or external factors impacting pickup/drop timing.</li>
  <li><strong>Customer Support:</strong> For assistance, please contact our helpline: +91 7065 650 650.</li>
</ul>

      </div>
    <div style="text-align: center;">
      <img src="./assets/footer-ticket.png" alt="footer" width="100%">
    </div>
    </div>
  </div>



  <button class="download-btn" onclick="generatePDF()" style="margin-bottom: 10px;">Download Ticket</button>

  <script>
    function generatePDF() {
      const element = document.getElementById('ticket');
      html2pdf()
        .set({
          margin: 0,
          filename: 'GoToGo-Ticket.pdf',
          image: { type: 'jpeg', quality: 0.98 },
          html2canvas: { scale: 2, useCORS: true },
          jsPDF: {
            unit: 'px',
            format: [375, 667],
            orientation: 'portrait'
          }
        })
        .from(element)
        .save();
    }
  </script>

</body>
</html>




<!-- 
<script>
      function generateTicketNumber() {
        const now = new Date();
        let hours = now.getHours();
        const minutes = now.getMinutes();

        const period = hours >= 12 ? "PM" : "AM";
        hours = hours % 12 || 12;
        const hourStr = hours.toString().padStart(2, "0");
        const minuteStr = minutes.toString().padStart(2, "0");

        const timePart = `${hourStr}${minuteStr}`;
        const random = Math.floor(100 + Math.random() * 900);

        return `G2G-${period}-${timePart}-${random}`;
      }

      function updateCheckoutSummary() {
        const names = [];
        const serviceType = document.querySelector(
          'input[name="serviceType"]:checked'
        )?.value;

        for (let i = 1; i <= 5; i++) {
          const name = document.getElementById(`name${i}`).value.trim();
          if (name) names.push(name);
        }

        let price = 0;
        if (serviceType === "Shuttle") {
          price = names.length * 10;
        } else if (serviceType === "Sedan") {
          if (names.length > 3) {
            showSedanModal(); // Show modal instead of alert
            return;
          }
          price = 40;
        } else if (serviceType === "SUV") {
          if (names.length > 5) {
            showCallModal(); // You can show same modal or a different one for SUV
            return;
          }
          price = 50;
        }

        const checkoutElement = document.getElementById("checkout");
        if (serviceType && names.length > 0) {
          checkoutElement.innerHTML = `<strong>${names.length} Seat${
            names.length > 1 ? "s" : ""
          } on ${serviceType} Drop @ $${price}</strong>`;
        } else {
          checkoutElement.innerHTML = "";
        }
      }

      document.addEventListener("DOMContentLoaded", () => {
        const bookingForm = document.getElementById("bookingForm");

        // ✅ LIVE UPDATE LOGIC
        for (let i = 1; i <= 5; i++) {
          document
            .getElementById(`name${i}`)
            .addEventListener("input", updateCheckoutSummary);
        }

        document
          .querySelectorAll('input[name="serviceType"]')
          .forEach((input) =>
            input.addEventListener("change", updateCheckoutSummary)
          );

        updateCheckoutSummary();

        bookingForm.addEventListener("submit", async function (e) {
          e.preventDefault();

          // ✅ Find the button
          const payBtn = document.getElementById("submitBooking");

          // ✅ Show loader and disable button
          payBtn.disabled = true;
          payBtn.innerHTML = `
    <div style="display: inline-flex; align-items: center;">
      <div class="spinner" style="
        width: 18px;
        height: 18px;
        border: 3px solid #f3f3f3;
        border-top: 3px solid white;
        border-radius: 50%;
        margin-right: 8px;
        animation: spin 0.8s linear infinite;
      "></div>
      Wait a while we are Processing...
    </div>
  `;

          // ✅ Add CSS for the loader (if not added already)
          if (!document.getElementById("btn-spinner-style")) {
            const style = document.createElement("style");
            style.id = "btn-spinner-style";
            style.textContent = `
      @keyframes spin {
        0% { transform: rotate(0deg); }
        100% { transform: rotate(360deg); }
      }
    `;
            document.head.appendChild(style);
          }

          const names = [];
          const phones = [];

          for (let i = 1; i <= 5; i++) {
            const name = document.getElementById(`name${i}`).value.trim();
            const code = document.getElementById(`code${i}`).value.trim();
            const phone = document.getElementById(`phone${i}`).value.trim();

            if (name) names.push(name);
            if (phone) phones.push(`${code} ${phone}`);
          }

          const pickupDate = document.getElementById("pickupDate").value;
          const pickupLocation = document
            .getElementById("pickupLocation")
            .value.trim();
          const boardingTime = document.getElementById("boardingTime").value;
          const terminal = document.getElementById("dropTerminal").value.trim();
          const serviceType = document.querySelector(
            'input[name="serviceType"]:checked'
          )?.value;
          const email = document.getElementById("email")?.value.trim(); // ✅ Fetch from input field
          const ticketNumber = generateTicketNumber();

          if (
            !pickupDate ||
            !pickupLocation ||
            !boardingTime ||
            !terminal ||
            !serviceType
          )
            return alert("Please fill all required fields.");
          if (names.length === 0)
            return alert("At least one passenger name is required.");
          if (phones.length < names.length)
            return alert("Please fill valid phone numbers for all passengers.");
          if (!email || !email.includes("@"))
            return alert("Please enter a valid email.");

          const today = new Date().toISOString().split("T")[0];
          if (pickupDate < today)
            return alert("Pickup date cannot be in the past.");

          let price = 0;

          if (serviceType === "Shuttle") {
            price = 10 * names.length;
          } else if (serviceType === "Sedan") {
            if (names.length > 3) return alert("Max 3 passengers for Sedan.");
            price = 40;
          } else if (serviceType === "SUV") {
            if (names.length > 5) return alert("Max 5 passengers for SUV.");
            price = 50;
          }

          let priceInINR = price;

          try {
            const res = await fetch(
              "https://v6.exchangerate-api.com/v6/5a2fbf556551938d74d19597/latest/USD"
            );
            const data = await res.json();

            const rate = data?.conversion_rates?.INR;

            if (!rate) throw new Error("INR rate missing in API response");

            priceInINR = Math.round(price * rate);

            console.log(`💱 USD to INR rate: ₹${rate}`);
            console.log(`💰 Final Price in INR: ₹${priceInINR}`);
          } catch (err) {
            console.error("❌ Failed to convert USD to INR:", err.message);
            alert("Failed to fetch currency exchange rate. Please try again.");
            return;
          }

          // alert(`💰 Amount to be paid: ₹${price}`);

          try {
            const orderRes = await fetch(
              "https://testpayment-iuah.onrender.com/api/create-order",
              {
                method: "POST",
                headers: { "Content-Type": "application/json" },
                body: JSON.stringify({ amount: priceInINR }),
              }
            );

            const orderData = await orderRes.json();

            if (!orderData.id)
              return alert("❌ Order creation failed. Please try again.");

            const bookingData = {
              names,
              phones,
              pickupDate,
              pickupLocation,
              boardingTime,
              terminal,
              serviceType,
              amountPaid: priceInINR,
              ticketNumber: ticketNumber,
            };

            const razorpayOptions = {
              key: "rzp_test_7m2jpATTXnOo2o", // Replace with your real Razorpay key
              amount: orderData.amount,
              currency: "USD",
              order_id: orderData.id,
              name: "GoToGo Airport Shuttle",
              description: "Booking Payment",
              handler: async function (response) {
                console.log("🎯 Razorpay Response:", response);

                const verifyRes = await fetch(
                  "https://testpayment-iuah.onrender.com/verify",
                  {
                    method: "POST",
                    headers: { "Content-Type": "application/json" },
                    body: JSON.stringify({
                      razorpay_order_id: response.razorpay_order_id,
                      razorpay_payment_id: response.razorpay_payment_id,
                      razorpay_signature: response.razorpay_signature,
                      bookingData,
                      email,
                    }),
                  }
                );

                const verifyResult = await verifyRes.json();
                console.log("📩 Verify API Response:", verifyResult);

                if (verifyResult.success) {
                  if (!response || !response.razorpay_payment_id) {
                    console.error("❌ Missing Razorpay Payment ID");
                    return alert("Something went wrong! Missing payment ID.");
                  }

                  bookingData.paymentId = response.razorpay_payment_id;

                  try {
                    // Save to localStorage
                    localStorage.setItem(
                      "bookingDetails",
                      JSON.stringify(bookingData)
                    );
                    console.log("✅ Booking data saved to localStorage.");

                    // ✅ Show loader + message before redirection
                    const loaderDiv = document.createElement("div");
                    loaderDiv.style.cssText = `
      position: fixed;
      top: 0; left: 0;
      width: 100vw; height: 100vh;
      background: rgba(255, 255, 255, 0.95);
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      z-index: 9999;
    `;
                    loaderDiv.innerHTML = `
      <div class="spinner" style="
        border: 6px solid #f3f3f3;
        border-top: 6px solid #0c52a2;
        border-radius: 50%;
        width: 50px;
        height: 50px;
        animation: spin 1s linear infinite;
      "></div>
      <p style="margin-top: 20px; font-size: 18px; color: #0c52a2;">Please wait while we generate your ticket...</p>
    `;
                    document.body.appendChild(loaderDiv);

                    // Spinner animation keyframe (add once)
                    const style = document.createElement("style");
                    style.innerHTML = `
      @keyframes spin {
        0% { transform: rotate(0deg); }
        100% { transform: rotate(360deg); }
      }
    `;
                    document.head.appendChild(style);

                    // ✅ Wait 1 second before redirect
                    setTimeout(() => {
                      window.location.href = "your-ticket.html";
                    }, 1200);
                  } catch (err) {
                    console.error("❌ Failed to save booking data:", err);
                    alert(
                      "Could not save your booking. Please contact our support team at 7065650650."
                    );
                  }
                } else {
                  alert(
                    "❌ Payment verification failed! Reason: " +
                      (verifyResult.error || "Unknown error")
                  );
                }
              },
              prefill: {
                name: names[0],
                contact: phones[0],
              },
              theme: { color: "#0c52a2" },
            };

            const rzp = new Razorpay(razorpayOptions);
            rzp.open();
          } catch (err) {
            console.error(err);
            alert("❌ Something went wrong during payment process.");
          }
        });
      });
    </script> -->