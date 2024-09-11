# Danh sách sản phẩm
products = [
    {"name": "Laptop", "price": 1000, "quantity": 2},
    {"name": "Mouse", "price": 25, "quantity": 5},
    {"name": "Keyboard", "price": 50, "quantity": 3},
]

# Hàm tính tổng tiền của sản phẩm
def calculate_total(products):
    total = 0
    print("Tổng hợp sản phẩm:")
    for product in products:
        product_total = product["price"] * product["quantity"]
        print(f"Sản phẩm: {product['name']} - Giá: {product['price']} - Số lượng: {product['quantity']} - Tổng tiền: {product_total}")
        total += product_total
    return total

# Tính và in tổng tiền
total_price = calculate_total(products)
print(f"Tổng tiền tất cả sản phẩm: {total_price}")
