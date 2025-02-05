# Understanding JavaScript Object Literals

Object literals in JavaScript are a simple yet powerful way to store and manage data using key-value pairs. They are widely used in web development for handling structured information.

## 📌 Defining an Object
```javascript
const post = {
    username: "rana_nikhil_singh_",
    post_id: "1234567890",
    post_content: "Hello, I am Nikhil Singh",
    likes: 50,
    comments: 20,
    tags: ["@nikhilsingh"]
};
```

## 📌 Accessing Properties
```javascript
console.log(post.username); // rana_nikhil_singh_
console.log(post["post_content"]); // Hello, I am Nikhil Singh
```

## 📌 Converting Retrieved Values
```javascript
console.log(String(post.likes)); // Converts number to string
console.log(Boolean(post.comments)); // Converts number to boolean
```

## 📌 Modifying an Object
### Adding a Property
```javascript
post.shares = 10; 
console.log(post);
```

### Updating a Property
```javascript
post.likes += 10; 
console.log(post);
```

### Removing a Property
```javascript
delete post.post_id;
console.log(post);
```

## 📌 Working with Nested Objects
```javascript
const user = {
    name: "Nikhil Singh",
    profile: {
        age: 22,
        location: "India",
        profession: "Developer"
    }
};

console.log(user.profile.location); // India
```

## 📌 Using an Array of Objects
```javascript
const posts = [
    { username: "rana_nikhil_singh_", post_content: "Exploring JavaScript!", likes: 50 },
    { username: "coder_amit", post_content: "Learning Objects in JS!", likes: 75 }
];

console.log(posts[1].post_content); // Learning Objects in JS!
