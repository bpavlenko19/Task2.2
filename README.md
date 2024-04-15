# Task2.2
from flask import Flask, request, jsonify

app = Flask(__name__)

@app.route('/login', methods=['POST'])
def login_user():
    # Реалізація аутентифікації користувача
    return jsonify({'message': 'Login successful'}), 200

if __name__ == '__main__':
    app.run(port=5002)
