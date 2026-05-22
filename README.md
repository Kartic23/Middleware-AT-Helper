## 🧰 Middleware AT Helper

Middleware AT Helper is a lightweight web tool designed to simplify the handling of fiscal and middleware payloads.

### ✨ Features

- Convert Base64-encoded PDF data into downloadable PDF files
- Support for full JSON payloads (automatically extracts the PDF and document name)
- Direct Base64 input option
- Automatic file naming based on `DocumentNumber`
- Input validation and error handling
- Clean and user-friendly green-themed UI

### 📦 Supported Payload Format

The tool accepts structured JSON responses that include a Base64-encoded PDF, such as:

```json
{
    "DocumentNumber": "ZGAC DLOSSJKLD/5",
    "ATCUD": "PSLPSLCPP-5",
    "ATDocCodeID": "1107986025",
    "StatusCode": 200,
    "StatusMessage": "Alerta: Erro na validação do ATCUD. Campos número de documento e ATCUD com erros ou incompletos.",
    "PDF": "BASE64_STRING"
}
