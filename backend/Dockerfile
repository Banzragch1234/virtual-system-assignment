FROM node:18-alpine AS builder
WORKDIR /app
RUN touch my-app.js

FROM alpine:3.18
WORKDIR /app
COPY --from=builder /app/my-app.js .
CMD ["sh", "-c", "echo 'Backend Multi-stage Build амжилттай!' && tail -f /dev/null"]
