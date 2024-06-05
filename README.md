create TABLE barang(
barangID INT NOT NULL AUTO_INCREMENT,
barangName VARCHAR(100) NOT NULL,
barangHarga FLOAT(40) NOT NULL,
barangStock INT,
PRIMARY KEY ( barangID )
);

DROP table barang;

INSERT INTO barang ( barangName, barangHarga,barangStock )
VALUES
("Handphone",20000,4),
("Laptop",80000,2),
("Televisi",50000,6);

SELECT barangName, barangHarga FROM barang

SELECT * FROM barang
WHERE barangstock < 5;

SELECT * FROM barang
WHERE barangName = "Laptop";

UPDATE barang SET barangName = 'LaptopPutih' WHERE barangID = 2;

SELECT * FROM barang
WHERE barangName LIKE "Han%";

