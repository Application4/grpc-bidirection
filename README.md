# grpc-bidirection

You and your friend keep roasting each other at the same time. Infinite back and forth. Fun until someone gets hurt. 😆

liveTrading

grpcurl -d @ \
  -plaintext \
  -import-path ~/Downloads/grpc-unary-server/src/main/proto \
  -proto stock_trading.proto \
  localhost:9090 \
  stocktrading.StockTradingService/LiveTrading < order.txt
