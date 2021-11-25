const ticketWeightFunction = (address, stake, price, sTokens, a, b) => {
  if (price > stake) {
    return 'Stake Price Required to be Higher than Price of Item';
  }
  let ticket = {};
  let ticketWeight = (stake/price)**a * (sTokens + 1)**b;
  ticket[address] = ticketWeight;
  return ticket;
}

/*
//The following variables come from Participant input to Smart Contract
address = '0x1234567890';
stake = 450;
sTokens = 5;
//The following variables come from Sponsor parameters
price = 450;
a = 3;
b = 1.2;

let ticketWeightFactor = ticketWeightFunction(address, stake, price, sTokens, a, b);
*/

module.exports = ticketWeightFunction;
