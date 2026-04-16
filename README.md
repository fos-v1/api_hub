# Freightoscope Swagger Portal

This folder contains a Swagger UI portal for the Freightoscope and FOS Connect APIs.

## Included specs

- `specs/inquiry-new-rate-request.yaml`: New Rate Request API for input into Freightoscope
- `specs/inquiry-rate-request-email-ai-processing.yaml`: Rate Request Email AI processing API for output from Freightoscope
- `specs/quotation.yaml`: Freightoscope quotation retrieval API
- `specs/customer-booking.yaml`: Freightoscope customer booking retrieval API
- `specs/financial-documents.yaml`: Freightoscope outbound financial document APIs for invoice, credit note, debit note, and bill posting
- `specs/fos-connect.yaml`: FOS Connect APIs copied from the existing project spec and sanitized for documentation use
- `specs/shipment.yaml`: Freightoscope shipment APIs with GET and POST endpoints for air, sea, and inland shipments

## Local preview

Use a simple local HTTP server so Swagger UI can fetch the YAML files:

```bash
python -m http.server 8000
```

Then open:

```text
http://localhost:8000/api_hub/
```

## Notes

- The original text files were left untouched.
- Placeholder credentials are used in the published specs.
- You can add more FOS Connect specs later and wire them into `index.html`.
