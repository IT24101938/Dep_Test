backend/models
const ItemSchema = new mongoose.Schema({
    name: { type: String, required: true },
    price: {type: Number, required: true},
    discountPercentage: {type: Number, required: true}
    
}, { timestamps: true });

backend/routes
// POST create item
router.post('/', async (req, res) => {
  const item = new Item({
    name: req.body.name,
    price: req.body.price,
    discountPercentage: req.body.discountPercentage
    // will work once you add price to the model
  });

frontend/components/ItemForm.jsx
const handleSubmit = async (e) => {
    e.preventDefault();

    await createItem({
      name,
      price: Number(price),
      discountPercentage: Number(discountPercentage)
  
});

    setName('');
    setPrice('');
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
          <p>{item.description}</p>
          <p>Price: Rs.{item.price}</p>
          <p>Discount: {item.discountPercentage}%</p>

Github Commands
echo "# aa" >> README.md
git init
git add README.md
git add .
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/IT24101938/Dep_Test.git
git push -u origin main
