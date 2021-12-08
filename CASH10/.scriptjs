const billAmount = document.querySelector("#bill-amount");
const cashGiven = document.querySelector("#cash-given");
const checkButton = document.querySelector("#check-button");
const message = document.querySelector("#error-message");
const noOfNotes = document.querySelectorAll(".no-of-notes")
const availableNotes = [2000, 500, 100, 20, 10, 5, 1];
checkButton.addEventListener("click", function validateBillAndCashAmount() {
    hideMessage();
    message.style.display = "none";
    if (billAmount.value > 0) {
        if (cashGiven.value >= billAmount.value) {

            const amountToBeReturn = cashGiven.value - billAmount.value;
            calculateChange(amountToBeReturn);
        } else {
            showMessage("Do you wanna wash the glasses?");

        }

    } else {
        showMessage("Invalid Bill Amount")

    }
});

function calculateChange(amountToBeReturn) {
    for (i = 0; i < availableNotes.length; i++) {
        constnumberOfNotes = Math.trunc(
            amountToBeReturn / availableNotes[i]
        );
        amountToBeReturn %= availableNotes[i];
        noOfNotes[i].innerText = numberOfNotes;

    };
};

function hideMessage() {
    message.style.display = "none";
}

function showMessage(msg) {
    // console.log("here");
    message.style.display = "block";
    message.innerText = msg;
}
checkButton.addEventListener("click", calculateChange);