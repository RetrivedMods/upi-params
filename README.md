# UPI Parameters

A reference for UPI deep link parameters used in payment URLs, QR codes, and merchant integrations.

## Basic Format

```text
upi://pay?pa=payee@upi&pn=Payee&am=100&cu=INR
```

## Parameters

| Parameter | Description |
|------------|------------|
| pa | Payee UPI ID (VPA) |
| pn | Payee Name |
| am | Amount |
| cu | Currency |
| tn | Transaction Note |
| tr | Transaction Reference |
| tid | Transaction ID |
| mc | Merchant Category Code |
| url | Merchant Website URL |
| mam | Minimum Amount |
| mode | Payment Mode |
| purpose | Purpose Code |
| orgid | Organization ID |
| sign | Digital Signature |
| mid | Merchant ID |
| msid | Merchant Store ID |
| mtid | Merchant Terminal ID |
| gstBrkUp | GST Breakdown |
| gstIn | GST Number |
| invoiceNo | Invoice Number |
| invoiceDate | Invoice Date |
| refUrl | Reference URL |

## Example

```text
upi://pay?pa=nics@upi&pn=Nics&am=99&cu=INR&tn=Premium
```

## Full Example

```text
upi://pay?pa=nics@upi
&pn=Nics
&am=99
&cu=INR
&tn=Premium Subscription
&tr=TXN001
&tid=TXN001
&mc=1234
&url=https://example.com
&mam=1
&mode=01
&purpose=00
&orgid=123456
```

## Notes

- Currency is typically `INR`.
- Parameter support may vary across UPI apps and PSPs.
- Some parameters are merchant-specific and may not be supported by all apps.
- Unknown parameters are usually ignored by UPI applications.

## Contributing

Found a missing parameter or field? Open a pull request.

## License

MIT
