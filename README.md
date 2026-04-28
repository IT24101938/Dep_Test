backend/models
const ItemSchema = new mongoose.Schema({
    name: { type: String, required: true },
    discountPercentage: {type: Number, required: true}
}, { timestamps: true });

backend/routes
// POST create item
router.post('/', async (req, res) => {
  const item = new Item({
    name: req.body.name,
    discountPercentage: req.body.discountPercentage
});

frontend/components/ItemForm.jsx
const handleSubmit = async (e) => {
    e.preventDefault();

    await createItem({
      name,
      discountPercentage: Number(discountPercentage),
  
});

    setName('');
    setDiscountPercentage('');

    onItemAdded();
  };

      <div>
        <input
          placeholder="Description"
          value={description}
          onChange={(e) => setDescription(e.target.value)}
          required
        />
      </div>

      <div>
        <input
          placeholder="Price"
          type="number"
          value={price}
          onChange={(e) => setPrice(e.target.value)}
          required
        />
      </div>

frontend/components/ItemList.jsx
          <h3>{item.name}</h3>
          <p>Price: Rs.{item.price}</p>
          <p>Discount: {item.discountPercentage}%</p>

frontend/.env
MONGO_URI=mongodb+srv://lakindu:lakindu123@cluster1.o7igtj2.mongodb.net/?appName=Cluster1
PORT=5000

backend/.env
VITE_API_URL=http://localhost:5000/api

package.json
"scripts": {
    "start": "node server.js",
    "dev": "vite",
    "build": "vite build",
    "lint": "eslint .",
    "preview": "vite preview"
  },

Github Commands
echo "# aa" >> README.md
git init
git add README.md
git add .
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/IT24101938/Dep_Test.git
git push -u origin main
