<script>
export default {
    name:'MixCategory',
    data()
    {
        return{
            gridmenu:['All Product','T-Shirt','Hoodies','Jacket'],
            social:['facebook.png','twitter.png','linkedin.png','dribbble.png'],
            catelog:['Necklaces','Hoodies','Jewelry Box','T-Shirt','Jacket'],
            aboutus:['Our Producers','Sitemap','FAQx','About Us','Terms & Conditions'],
            newsletter:['i031.png','i0111.png','i071.png','i0121.png','i0141.png','i021.png'],
            customerservice:['Contact Us','Track Your Order','Product Care & Repairx','Book An Appointment','Shipping & Returns'],
            products:[
                {
                    name: 'Adicolor Classics Joggers',
                    image: 'p1.png',
                    type: 'Dress',
                    price:'63.85',
                    discount:null,
                    tag:null
                },
                {
                    name: 'Nike Sportswear Futura Luxee',
                    image: 'p2.png',
                    type: 'Bag',
                    price:'130.00',
                    discount:null,
                    tag:null
                },
                {
                    name: 'Geometric Print Scarf',
                    image: 'p3.png',
                    type: 'Scarf',
                    price:'53.00',
                    discount:null,
                    tag:null
                },
                {
                    name: 'Yellow Reserved Hoodie',
                    image: 'p4.png',
                    type: 'Dress',
                    price:'364.00',
                    discount:'155.00',
                    tag:'sale'
                },
                {
                    name: 'Basic Dress Green',
                    image: 'p5.png',
                    type: 'Dress',
                    price:'236.00',
                    discount:null,
                    tag:'hot'
                },
                {
                    name: 'Nike Air Zoom Pegasus',
                    image: 'p6.png',
                    type: 'Shoe',
                    price:'220.00',
                    discount:'198.00',
                    tag:'sale'
                },
                {
                    name: 'Nike Repel Miler',
                    image: 'p7.png',
                    type: 'Dress',
                    price:'120.50',
                    discount:null,
                    tag:null
                },
                {
                    name: 'Polarised Sunglasses',
                    image: 'p8.png',
                    type: 'Glasses',
                    price:'160.00',
                    discount:null,
                    tag:null
                },
                
            ]
        }
    }
}
</script>