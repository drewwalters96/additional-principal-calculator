# additional-principal-calculator

Calculator to determine additional principal needed to payoff loan by a certain year.

## Features

- **Interactive Loan Calculator**: Enter your loan details and see instant results
- **Visual Slider Interface**: Easily adjust your target payoff timeframe
- **Comprehensive Results**: View additional payment needed, years saved, and total interest saved
- **Responsive Design**: Works on desktop and mobile devices
- **No Dependencies**: Pure HTML, CSS, and JavaScript - no frameworks required

## Usage

Simply open `index.html` in your web browser to use the calculator.

### Input Fields

1. **Total Loan Amount ($)**: The principal amount of your loan
2. **Annual Interest Rate (%)**: Your loan's annual percentage rate (APR)
3. **Original Loan Term (Years)**: The original term of your loan in years
4. **New Payoff Timeframe (Years)**: Use the slider to select your desired payoff timeframe (1 year to original term)

### Results Displayed

- **Additional Monthly Payment Needed**: Extra amount to pay each month
- **Original Monthly Payment**: Standard payment for the original term
- **New Monthly Payment**: Total payment (original + additional)
- **Years Saved**: How many years earlier you'll pay off the loan
- **Total Interest Saved**: Total interest savings over the life of the loan

## Example

For a $300,000 loan at 4.5% interest with a 30-year term:
- **Paying off in 20 years instead**: Requires an additional $377.89/month
- **Savings**: 10 years earlier payoff and $91,712.58 in interest saved

## Technical Details

The calculator uses the standard amortization formula:
```
M = P * [r(1+r)^n] / [(1+r)^n - 1]
```

Where:
- M = Monthly payment
- P = Principal (loan amount)
- r = Monthly interest rate (annual rate / 12 / 100)
- n = Number of payments (years * 12)

## Local Development

To run locally:
```bash
# Start a simple web server (Python 3)
python3 -m http.server 8080

# Or with Node.js
npx http-server

# Then open http://localhost:8080 in your browser
```

## Browser Compatibility

Works with all modern browsers:
- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Opera (latest)

## License

MIT License - feel free to use and modify as needed.
