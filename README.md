# Currency-Converter
A currency converter that uses real-time exchange rates from an API.
# Currency Converter

## Description

A currency converter application that uses real-time exchange rates from an API.

## How to Run

1. **Replace API Key**:
    Replace `"your_api_key_here"` in `ExchangeRate.java` with your ExchangeRate-API key.

2. **Compile the Java files**:
    ```
    javac src/CurrencyConverter.java src/ConverterPanel.java src/ExchangeRate.java
    ```

3. **Run the CurrencyConverter**:
    ```
    java -cp src CurrencyConverter
    ```

4. **Follow the prompts**:
    - Enter an amount, select currencies from the drop-downs, and click on the "Convert" button.
    - The application will display the converted amount based on real-time exchange rates.

## Example Code

### ConverterPanel.java

```java
import javax.swing.*;
import java.awt.*;
import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;

public class ConverterPanel extends JPanel {
    private final JTextField amountField;
    private final JComboBox<String> fromCurrencyCombo;
    private final JComboBox<String> toCurrencyCombo;
    private final JLabel resultLabel;

    private static final String[] currencies = {"USD", "EUR", "GBP", "JPY", "CAD", "AUD"}; // Add more currencies as needed

    public ConverterPanel() {
        // Panel initialization code as shown previously
    }

    private class ConvertButtonListener implements ActionListener {
        // ActionListener implementation as shown previously
    }

    private double convertCurrency(double amount, String fromCurrency, String toCurrency) {
        // Method to convert currency using ExchangeRate.getExchangeRate as shown previously
    }
}
