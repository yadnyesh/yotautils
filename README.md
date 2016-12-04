# yotautils

var formatPrice = function (price) {
	const options = {style: 'currency', currency: 'INR'};
	const rupees = price / 100;

	if(rupees % 1 == 0) options.maximumSignificantDigits = 0;

	return rupees.toLocaleString('en-IN', options);
}

formatPrice (1010);
