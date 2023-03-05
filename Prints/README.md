# 3D Prints

## Slicer Profiles

Slicer profiles can be found in the `Slicer Profiles` directory.

## Ready-to-print Files

All files under this directory follows the naming rule:

```
VEMML-[version]-[varient]-[machine][-material][-batch]
```

- `[version]`: such as `v0_2`.
- `[varient]`: a short varient code, see the [Varient Codes](#varient-codes) section below for a reference table.
- `[machine]`: a code that represents the 3D printing machine, see the [Machines](#machines) section below for a reference table.
- `[-material]`: a code that represents the filament or resin, see the [Materials](#materials) section below for a reference table. Some files are generic according to the material used, and they will not contain this part in their filename.
- `[-batch]`: some printers require mutiple batches to print all the parts needed, in such case this part will be like `x_of_y`. Some batch may need to be printed mutiple times to get all the parts needed, for those batchs a `t_z` will be added, such as `1_of_3_t_2` means that this batch should be printed 2 times.

Examples:

* `VEMML-v0_2-A001-PN4K-OP410-1_of_3_t_2`

### Varient Codes

- UPERFECT 13.3" 4K (T10 R6.4 SD-15 BD-15) on MacBook Air 2020: `A001`, if there's no `A001` then use `0000`

### Machines

- `PN4K`: Phrozen Sonic Mini 4K
- `S2A2`: Snapmaker 2.0 A250

#### More info

##### Phrozen Sonic Mini 4K

3 batches: 

1. One leg with other parts
2. Main body (left)
3. Main body (right)

First batch need to print 2 times since we need 2 legs.

###### Limitations

Can only print legs less than 270mm long.

### Materials

- `OP410`: Onyx Rigid Pro410 Resin
- `PRS`: Phrozen Rock-Black Stiff Resin
- `SPLA`: Snapmaker PLA 
- `STPU` Snapmaker TPU
