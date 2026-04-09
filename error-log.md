1.Test lỗi bỏ trống dữ liệu (Vi phạm NOT NULL):
ERROR:  null value in column "name" of relation "products" violates not-null constraint
DETAIL:  Failing row contains (3, null, 100.00, 10, 2026-04-09 12:33:48.939606).
2.est lỗi tồn kho âm (Vi phạm CHECK stock):
ERROR:  new row for relation "products" violates check constraint "products_stock_check"
DETAIL:  Failing row contains (4, Tai nghe xịn, 200.00, -5, 2026-04-09 12:33:59.756961).
3.Test lỗi trùng lặp dữ liệu (Vi phạm PRIMARY KEY):
ERROR:  duplicate key value violates unique constraint "products_pkey"
DETAIL:  Key (id)=(1) already exists.