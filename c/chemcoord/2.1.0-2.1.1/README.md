# Comparing `tmp/chemcoord-2.1.0.tar.gz` & `tmp/chemcoord-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chemcoord-2.1.0.tar", last modified: Fri Aug  4 14:13:29 2023, max compression
+gzip compressed data, was "chemcoord-2.1.1.tar", last modified: Tue May  7 13:59:41 2024, max compression
```

## Comparing `chemcoord-2.1.0.tar` & `chemcoord-2.1.1.tar`

### file list

```diff
@@ -1,192 +1,192 @@
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-08-04 14:13:29.989633 chemcoord-2.1.0/
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      905 2023-08-04 13:10:33.000000 chemcoord-2.1.0/CHANGELOG.md
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     7644 2023-06-19 10:17:01.000000 chemcoord-2.1.0/LICENSE.md
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)       77 2023-06-19 10:17:01.000000 chemcoord-2.1.0/MANIFEST.in
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     5858 2023-08-04 14:13:29.989633 chemcoord-2.1.0/PKG-INFO
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     4766 2023-08-02 12:14:08.000000 chemcoord-2.1.0/README.rst
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-08-04 14:13:29.973633 chemcoord-2.1.0/docs/
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-08-04 14:13:29.973633 chemcoord-2.1.0/docs/source/
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      546 2023-08-02 12:14:08.000000 chemcoord-2.1.0/docs/source/bugs.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      965 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/cartesian_coordinates.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     1081 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/configuration.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      190 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/documentation.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      275 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/exceptions.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     2349 2023-08-02 12:14:08.000000 chemcoord-2.1.0/docs/source/index.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      844 2023-08-02 12:14:08.000000 chemcoord-2.1.0/docs/source/installation.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      690 2023-08-02 12:14:08.000000 chemcoord-2.1.0/docs/source/internal_coordinates.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     7445 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/license.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     1381 2023-08-02 12:14:08.000000 chemcoord-2.1.0/docs/source/references.rst
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-08-04 14:13:29.973633 chemcoord-2.1.0/docs/source/src_AsymmetricUnitCartesian/
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      258 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_AsymmetricUnitCartesian/chemcoord.AsymmetricUnitCartesian.rst
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-08-04 14:13:29.973633 chemcoord-2.1.0/docs/source/src_AsymmetricUnitCartesian/src_AsymmetricUnitCartesian/
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      180 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_AsymmetricUnitCartesian/src_AsymmetricUnitCartesian/chemcoord.AsymmetricUnitCartesian.get_cartesian.rst
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-08-04 14:13:29.973633 chemcoord-2.1.0/docs/source/src_Cartesian/
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     3039 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/chemcoord.Cartesian.rst
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-08-04 14:13:29.981633 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      135 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.__init__.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      160 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian._divide_et_impera.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      152 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian._preserve_bonds.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      129 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.add_data.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      118 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.align.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      121 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.append.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      145 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.basistransform.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      153 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.change_numbering.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      164 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.check_absolute_refs.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      147 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.check_dihedral.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      127 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.columns.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      115 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.copy.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      170 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.correct_absolute_refs.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      153 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.correct_dihedral.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      135 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.cut_cuboid.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      135 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.cut_sphere.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      136 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.fragmentate.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      149 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.from_ase_atoms.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      173 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.from_pymatgen_molecule.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      158 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_angle_degrees.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      146 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_ase_atoms.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      164 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_asymmetric_unit.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      147 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_barycenter.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      155 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_bond_lengths.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      132 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_bonds.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      141 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_centroid.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      173 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_construction_table.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      176 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_coordination_sphere.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      167 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_dihedral_degrees.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      152 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_distance_to.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      164 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_electron_number.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      167 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_equivalent_atoms.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      141 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_fragment.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      138 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_grad_zmat.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      138 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_inertia.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      147 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_pointgroup.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      170 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_pymatgen_molecule.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      170 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_shortest_distance.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      149 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_total_mass.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      138 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_without.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      129 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_zmat.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      118 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.iloc.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      121 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.index.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      121 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.insert.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      115 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.loc.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      161 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.partition_chem_env.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      135 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.read_cjson.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      129 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.read_xyz.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      150 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.reindex_similar.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      124 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.replace.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      161 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.restrict_bond_dict.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      132 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.set_index.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      135 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.sort_index.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      138 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.sort_values.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      115 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.subs.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      133 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.symmetrize.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      129 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.to_cjson.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      129 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.to_latex.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      132 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.to_string.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      123 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.to_xyz.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      126 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.to_zmat.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      115 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.view.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      132 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.write_xyz.rst
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-08-04 14:13:29.981633 chemcoord-2.1.0/docs/source/src_PointGroupOperations/
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      132 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_PointGroupOperations/chemcoord.PointGroupOperations.rst
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-08-04 14:13:29.981633 chemcoord-2.1.0/docs/source/src_Zmat/
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     1204 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/chemcoord.Zmat.rst
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-08-04 14:13:29.985633 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      120 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.__init__.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      114 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.add_data.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      138 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.change_numbering.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      112 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.columns.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      100 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.copy.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      109 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.dtypes.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      129 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.get_cartesian.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      149 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.get_electron_number.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      138 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.get_grad_cartesian.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      134 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.get_total_mass.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      149 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.has_same_sumformula.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      103 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.iloc.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      106 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.index.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      106 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.insert.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      112 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.iupacify.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      100 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.loc.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      144 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.minimize_dihedrals.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      117 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.read_zmat.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      120 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.safe_iloc.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      117 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.safe_loc.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      106 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.shape.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      120 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.sort_index.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      123 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.sort_values.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      100 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.subs.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      114 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.to_latex.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      117 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.to_string.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      108 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.to_xyz.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      111 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.to_zmat.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      126 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.unsafe_iloc.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      123 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.unsafe_loc.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      103 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.write.rst
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-08-04 14:13:29.985633 chemcoord-2.1.0/docs/source/src_configuration/
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      182 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_configuration/chemcoord.configuration.read_configuration_file.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      185 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_configuration/chemcoord.configuration.write_configuration_file.rst
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-08-04 14:13:29.985633 chemcoord-2.1.0/docs/source/src_exceptions/
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      183 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_exceptions/chemcoord.exceptions.IllegalArgumentCombination.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      153 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_exceptions/chemcoord.exceptions.InvalidReference.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      150 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_exceptions/chemcoord.exceptions.PhysicalMeaning.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      180 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_exceptions/chemcoord.exceptions.UndefinedCoordinateSystem.rst
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-08-04 14:13:29.985633 chemcoord-2.1.0/docs/source/src_xyz_functions/
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      143 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_xyz_functions/chemcoord.xyz_functions.allclose.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      179 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_xyz_functions/chemcoord.xyz_functions.apply_grad_zmat_tensor.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      137 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_xyz_functions/chemcoord.xyz_functions.concat.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      128 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_xyz_functions/chemcoord.xyz_functions.dot.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      140 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_xyz_functions/chemcoord.xyz_functions.isclose.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      154 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_xyz_functions/chemcoord.xyz_functions.read_molden.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      148 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_xyz_functions/chemcoord.xyz_functions.to_molden.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      131 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_xyz_functions/chemcoord.xyz_functions.view.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      157 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_xyz_functions/chemcoord.xyz_functions.write_molden.rst
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-08-04 14:13:29.985633 chemcoord-2.1.0/docs/source/src_zmat_functions/
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      170 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_zmat_functions/chemcoord.zmat_functions.DummyManipulation.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      176 2023-08-02 12:14:08.000000 chemcoord-2.1.0/docs/source/src_zmat_functions/chemcoord.zmat_functions.PureInternalMovement.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      158 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_zmat_functions/chemcoord.zmat_functions.TestOperators.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      197 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_zmat_functions/chemcoord.zmat_functions.apply_grad_cartesian_tensor.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      896 2023-08-04 13:10:33.000000 chemcoord-2.1.0/docs/source/tutorial.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)       38 2023-08-04 14:13:29.989633 chemcoord-2.1.0/setup.cfg
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     1978 2023-08-04 13:10:33.000000 chemcoord-2.1.0/setup.py
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-08-04 14:13:29.973633 chemcoord-2.1.0/src/
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-08-04 14:13:29.985633 chemcoord-2.1.0/src/chemcoord/
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     1187 2023-08-04 14:06:41.000000 chemcoord-2.1.0/src/chemcoord/__init__.py
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-08-04 14:13:29.985633 chemcoord-2.1.0/src/chemcoord/_generic_classes/
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-06-19 10:17:01.000000 chemcoord-2.1.0/src/chemcoord/_generic_classes/__init__.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      490 2023-08-02 12:14:08.000000 chemcoord-2.1.0/src/chemcoord/_generic_classes/generic_IO.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     3058 2023-08-02 12:14:08.000000 chemcoord-2.1.0/src/chemcoord/_generic_classes/generic_core.py
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-08-04 14:13:29.989633 chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-06-19 10:17:01.000000 chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/__init__.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    49583 2023-08-02 12:14:08.000000 chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/_cart_transformation.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    52210 2023-08-02 12:14:08.000000 chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/_cartesian_class_core.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    32040 2023-08-04 12:49:57.000000 chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/_cartesian_class_get_zmat.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    14387 2023-08-02 12:14:08.000000 chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/_cartesian_class_io.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    10567 2023-08-04 12:49:57.000000 chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/_cartesian_class_pandas_wrapper.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     4671 2023-08-02 12:14:08.000000 chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/_cartesian_class_symmetry.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     1641 2023-08-02 12:14:08.000000 chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/_indexers.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     1411 2023-08-02 12:14:08.000000 chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/asymmetric_unit_cartesian_class.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     3277 2023-08-02 12:14:08.000000 chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/cartesian_class_main.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      989 2023-08-02 12:14:08.000000 chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/point_group.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    16332 2023-08-02 12:14:08.000000 chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/xyz_functions.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     3385 2023-06-19 10:17:01.000000 chemcoord-2.1.0/src/chemcoord/configuration.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    67997 2023-08-02 12:14:08.000000 chemcoord-2.1.0/src/chemcoord/constants.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     2257 2023-06-19 10:17:01.000000 chemcoord-2.1.0/src/chemcoord/exceptions.py
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-08-04 14:13:29.989633 chemcoord-2.1.0/src/chemcoord/internal_coordinates/
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-06-19 10:17:01.000000 chemcoord-2.1.0/src/chemcoord/internal_coordinates/__init__.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     2922 2023-08-02 12:14:08.000000 chemcoord-2.1.0/src/chemcoord/internal_coordinates/_indexers.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    30873 2023-08-04 12:49:57.000000 chemcoord-2.1.0/src/chemcoord/internal_coordinates/_zmat_class_core.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     7487 2023-08-04 12:49:57.000000 chemcoord-2.1.0/src/chemcoord/internal_coordinates/_zmat_class_io.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     3027 2023-08-02 12:14:08.000000 chemcoord-2.1.0/src/chemcoord/internal_coordinates/_zmat_class_pandas_wrapper.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     5573 2023-08-04 12:49:57.000000 chemcoord-2.1.0/src/chemcoord/internal_coordinates/_zmat_transformation.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     3182 2023-08-02 12:14:08.000000 chemcoord-2.1.0/src/chemcoord/internal_coordinates/zmat_class_main.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     4390 2023-08-02 12:14:08.000000 chemcoord-2.1.0/src/chemcoord/internal_coordinates/zmat_functions.py
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-08-04 14:13:29.989633 chemcoord-2.1.0/src/chemcoord/utilities/
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-06-19 10:17:01.000000 chemcoord-2.1.0/src/chemcoord/utilities/__init__.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     3365 2023-06-19 10:17:01.000000 chemcoord-2.1.0/src/chemcoord/utilities/_decorators.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     4591 2023-06-19 10:17:01.000000 chemcoord-2.1.0/src/chemcoord/utilities/_print_versions.py
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-08-04 14:13:29.985633 chemcoord-2.1.0/src/chemcoord.egg-info/
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     5858 2023-08-04 14:13:29.000000 chemcoord-2.1.0/src/chemcoord.egg-info/PKG-INFO
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    10517 2023-08-04 14:13:29.000000 chemcoord-2.1.0/src/chemcoord.egg-info/SOURCES.txt
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)        1 2023-08-04 14:13:29.000000 chemcoord-2.1.0/src/chemcoord.egg-info/dependency_links.txt
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)       77 2023-08-04 14:13:29.000000 chemcoord-2.1.0/src/chemcoord.egg-info/requires.txt
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)       10 2023-08-04 14:13:29.000000 chemcoord-2.1.0/src/chemcoord.egg-info/top_level.txt
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-07 13:59:41.052855 chemcoord-2.1.1/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      309 2024-05-06 18:47:43.000000 chemcoord-2.1.1/CHANGELOG.md
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     7644 2023-06-19 10:17:01.000000 chemcoord-2.1.1/LICENSE.md
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)       77 2023-06-19 10:17:01.000000 chemcoord-2.1.1/MANIFEST.in
+-rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)     6577 2024-05-07 13:59:41.052855 chemcoord-2.1.1/PKG-INFO
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     5169 2024-05-07 13:52:06.000000 chemcoord-2.1.1/README.rst
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-07 13:59:41.032854 chemcoord-2.1.1/docs/
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-07 13:59:41.032854 chemcoord-2.1.1/docs/source/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      858 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/bugs_and_contributors.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      965 2023-06-19 10:17:01.000000 chemcoord-2.1.1/docs/source/cartesian_coordinates.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     1081 2023-06-19 10:17:01.000000 chemcoord-2.1.1/docs/source/configuration.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      190 2023-06-19 10:17:01.000000 chemcoord-2.1.1/docs/source/documentation.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      275 2023-06-19 10:17:01.000000 chemcoord-2.1.1/docs/source/exceptions.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     3157 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/index.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     1079 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/installation.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      690 2023-08-02 12:14:08.000000 chemcoord-2.1.1/docs/source/internal_coordinates.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     7445 2023-06-19 10:17:01.000000 chemcoord-2.1.1/docs/source/license.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     1381 2023-08-02 12:14:08.000000 chemcoord-2.1.1/docs/source/references.rst
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-07 13:59:41.032854 chemcoord-2.1.1/docs/source/src_AsymmetricUnitCartesian/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     3330 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_AsymmetricUnitCartesian/chemcoord.AsymmetricUnitCartesian.rst
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-07 13:59:41.036855 chemcoord-2.1.1/docs/source/src_AsymmetricUnitCartesian/src_AsymmetricUnitCartesian/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      196 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_AsymmetricUnitCartesian/src_AsymmetricUnitCartesian/chemcoord.AsymmetricUnitCartesian.get_cartesian.rst
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-07 13:59:41.036855 chemcoord-2.1.1/docs/source/src_Cartesian/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     2291 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/chemcoord.Cartesian.rst
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-07 13:59:41.040855 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      145 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.__init__.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      170 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian._divide_et_impera.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      162 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian._preserve_bonds.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      139 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.add_data.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      128 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.align.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      155 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.basistransform.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      163 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.change_numbering.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      174 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.check_absolute_refs.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      157 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.check_dihedral.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      136 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.columns.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      125 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.copy.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      180 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.correct_absolute_refs.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      163 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.correct_dihedral.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      145 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.cut_cuboid.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      145 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.cut_sphere.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      146 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.fragmentate.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      159 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.from_ase_atoms.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      183 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.from_pymatgen_molecule.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      168 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_angle_degrees.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      156 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_ase_atoms.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      174 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_asymmetric_unit.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      157 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_barycenter.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      165 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_bond_lengths.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      142 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_bonds.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      151 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_centroid.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      183 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_construction_table.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      186 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_coordination_sphere.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      177 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_dihedral_degrees.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      162 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_distance_to.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      174 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_electron_number.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      177 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_equivalent_atoms.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      151 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_fragment.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      156 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_grad_zmat.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      148 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_inertia.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      157 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_pointgroup.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      180 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_pymatgen_molecule.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      180 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_shortest_distance.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      159 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_total_mass.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      148 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_without.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      139 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_zmat.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      127 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.iloc.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      130 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.index.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      131 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.insert.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      124 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.loc.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      171 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.partition_chem_env.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      145 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.read_cjson.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      139 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.read_xyz.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      160 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.reindex_similar.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      134 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.replace.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      171 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.restrict_bond_dict.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      142 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.set_index.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      145 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.sort_index.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      148 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.sort_values.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      125 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.subs.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      143 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.symmetrize.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      139 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.to_cjson.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      139 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.to_latex.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      142 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.to_string.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      133 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.to_xyz.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      136 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.to_zmat.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      125 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.view.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      142 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.write_xyz.rst
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-07 13:59:41.040855 chemcoord-2.1.1/docs/source/src_PointGroupOperations/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      651 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_PointGroupOperations/chemcoord.PointGroupOperations.rst
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-07 13:59:41.040855 chemcoord-2.1.1/docs/source/src_Zmat/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     1050 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/chemcoord.Zmat.rst
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-07 13:59:41.044855 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      130 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.__init__.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      124 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.add_data.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      148 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.change_numbering.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      121 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.columns.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      110 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.copy.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      118 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.dtypes.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      139 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.get_cartesian.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      159 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.get_electron_number.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      156 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.get_grad_cartesian.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      144 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.get_total_mass.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      160 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.has_same_sumformula.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      112 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.iloc.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      115 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.index.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      116 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.insert.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      122 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.iupacify.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      109 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.loc.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      154 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.minimize_dihedrals.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      127 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.read_zmat.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      129 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.safe_iloc.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      126 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.safe_loc.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      115 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.shape.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      130 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.sort_index.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      133 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.sort_values.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      110 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.subs.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      124 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.to_latex.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      127 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.to_string.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      118 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.to_xyz.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      121 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.to_zmat.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      135 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.unsafe_iloc.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      132 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.unsafe_loc.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      113 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.write.rst
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-07 13:59:41.044855 chemcoord-2.1.1/docs/source/src_configuration/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      189 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_configuration/chemcoord.configuration.read_configuration_file.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      192 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_configuration/chemcoord.configuration.write_configuration_file.rst
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-07 13:59:41.044855 chemcoord-2.1.1/docs/source/src_exceptions/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      183 2023-06-19 10:17:01.000000 chemcoord-2.1.1/docs/source/src_exceptions/chemcoord.exceptions.IllegalArgumentCombination.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      153 2023-06-19 10:17:01.000000 chemcoord-2.1.1/docs/source/src_exceptions/chemcoord.exceptions.InvalidReference.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      150 2023-06-19 10:17:01.000000 chemcoord-2.1.1/docs/source/src_exceptions/chemcoord.exceptions.PhysicalMeaning.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      180 2023-06-19 10:17:01.000000 chemcoord-2.1.1/docs/source/src_exceptions/chemcoord.exceptions.UndefinedCoordinateSystem.rst
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-07 13:59:41.048855 chemcoord-2.1.1/docs/source/src_xyz_functions/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      142 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_xyz_functions/chemcoord.xyz_functions.allclose.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      190 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_xyz_functions/chemcoord.xyz_functions.apply_grad_zmat_tensor.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      136 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_xyz_functions/chemcoord.xyz_functions.concat.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      127 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_xyz_functions/chemcoord.xyz_functions.dot.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      139 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_xyz_functions/chemcoord.xyz_functions.isclose.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      153 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_xyz_functions/chemcoord.xyz_functions.read_molden.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      147 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_xyz_functions/chemcoord.xyz_functions.to_molden.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      130 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_xyz_functions/chemcoord.xyz_functions.view.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      156 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_xyz_functions/chemcoord.xyz_functions.write_molden.rst
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-07 13:59:41.048855 chemcoord-2.1.1/docs/source/src_zmat_functions/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      310 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_zmat_functions/chemcoord.zmat_functions.DummyManipulation.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      322 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_zmat_functions/chemcoord.zmat_functions.PureInternalMovement.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      294 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_zmat_functions/chemcoord.zmat_functions.TestOperators.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      208 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_zmat_functions/chemcoord.zmat_functions.apply_grad_cartesian_tensor.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      896 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/tutorial.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)       38 2024-05-07 13:59:41.052855 chemcoord-2.1.1/setup.cfg
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     2122 2024-05-07 12:40:00.000000 chemcoord-2.1.1/setup.py
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-07 13:59:41.032854 chemcoord-2.1.1/src/
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-07 13:59:41.048855 chemcoord-2.1.1/src/chemcoord/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     1187 2023-08-04 15:24:20.000000 chemcoord-2.1.1/src/chemcoord/__init__.py
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-07 13:59:41.048855 chemcoord-2.1.1/src/chemcoord/_generic_classes/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-06-19 10:17:01.000000 chemcoord-2.1.1/src/chemcoord/_generic_classes/__init__.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      490 2023-08-02 12:14:08.000000 chemcoord-2.1.1/src/chemcoord/_generic_classes/generic_IO.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     3058 2023-08-04 15:24:20.000000 chemcoord-2.1.1/src/chemcoord/_generic_classes/generic_core.py
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-07 13:59:41.052855 chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-06-19 10:17:01.000000 chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/__init__.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    49629 2024-05-06 18:47:43.000000 chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/_cart_transformation.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    52118 2024-05-06 18:47:43.000000 chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/_cartesian_class_core.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    32242 2024-05-06 18:47:43.000000 chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/_cartesian_class_get_zmat.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    14356 2024-05-06 18:47:43.000000 chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/_cartesian_class_io.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    10567 2023-08-04 15:24:20.000000 chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/_cartesian_class_pandas_wrapper.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     4657 2024-05-06 18:47:43.000000 chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/_cartesian_class_symmetry.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     4092 2024-05-06 18:47:43.000000 chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/_indexers.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     1411 2023-08-02 12:14:08.000000 chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/asymmetric_unit_cartesian_class.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     3277 2023-08-02 12:14:08.000000 chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/cartesian_class_main.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      989 2023-08-02 12:14:08.000000 chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/point_group.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    16476 2024-05-06 18:47:43.000000 chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/xyz_functions.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     3385 2023-06-19 10:17:01.000000 chemcoord-2.1.1/src/chemcoord/configuration.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    67997 2023-08-04 15:24:20.000000 chemcoord-2.1.1/src/chemcoord/constants.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     2257 2023-06-19 10:17:01.000000 chemcoord-2.1.1/src/chemcoord/exceptions.py
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-07 13:59:41.052855 chemcoord-2.1.1/src/chemcoord/internal_coordinates/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-06-19 10:17:01.000000 chemcoord-2.1.1/src/chemcoord/internal_coordinates/__init__.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     4134 2024-05-06 18:47:43.000000 chemcoord-2.1.1/src/chemcoord/internal_coordinates/_indexers.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    31099 2024-05-06 18:47:43.000000 chemcoord-2.1.1/src/chemcoord/internal_coordinates/_zmat_class_core.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     7583 2024-05-06 18:47:43.000000 chemcoord-2.1.1/src/chemcoord/internal_coordinates/_zmat_class_io.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     3027 2023-08-02 12:14:08.000000 chemcoord-2.1.1/src/chemcoord/internal_coordinates/_zmat_class_pandas_wrapper.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     5573 2023-08-04 15:24:20.000000 chemcoord-2.1.1/src/chemcoord/internal_coordinates/_zmat_transformation.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     3182 2023-08-02 12:14:08.000000 chemcoord-2.1.1/src/chemcoord/internal_coordinates/zmat_class_main.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     4390 2023-08-02 12:14:08.000000 chemcoord-2.1.1/src/chemcoord/internal_coordinates/zmat_functions.py
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-07 13:59:41.052855 chemcoord-2.1.1/src/chemcoord/utilities/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-06-19 10:17:01.000000 chemcoord-2.1.1/src/chemcoord/utilities/__init__.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     3365 2023-06-19 10:17:01.000000 chemcoord-2.1.1/src/chemcoord/utilities/_decorators.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     4591 2023-06-19 10:17:01.000000 chemcoord-2.1.1/src/chemcoord/utilities/_print_versions.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      850 2024-05-06 18:47:43.000000 chemcoord-2.1.1/src/chemcoord/utilities/_temporary_deprecation_workarounds.py
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-07 13:59:41.052855 chemcoord-2.1.1/src/chemcoord.egg-info/
+-rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)     6577 2024-05-07 13:59:41.000000 chemcoord-2.1.1/src/chemcoord.egg-info/PKG-INFO
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    10525 2024-05-07 13:59:41.000000 chemcoord-2.1.1/src/chemcoord.egg-info/SOURCES.txt
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)        1 2024-05-07 13:59:41.000000 chemcoord-2.1.1/src/chemcoord.egg-info/dependency_links.txt
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)       77 2024-05-07 13:59:41.000000 chemcoord-2.1.1/src/chemcoord.egg-info/requires.txt
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)       10 2024-05-07 13:59:41.000000 chemcoord-2.1.1/src/chemcoord.egg-info/top_level.txt
```

### Comparing `chemcoord-2.1.0/LICENSE.md` & `chemcoord-2.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.0/PKG-INFO` & `chemcoord-2.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,56 @@
 Metadata-Version: 2.1
 Name: chemcoord
-Version: 2.1.0
+Version: 2.1.1
 Summary: Python module for dealing with chemical coordinates.
 Home-page: https://github.com/mcocdawc/chemcoord
 Author: Oskar Weser
 Author-email: oskar.weser@gmail.com
 License: LGPLv3
 Keywords: chemcoord,transformation,cartesian,internal,chemistry,zmatrix,xyz,zmat,coordinates,coordinate system
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
+Description-Content-Type: text/x-rst
 License-File: LICENSE.md
+Requires-Dist: numpy>=1.0
+Requires-Dist: scipy
+Requires-Dist: pandas>=1.0
+Requires-Dist: numba>=0.35
+Requires-Dist: sortedcontainers
+Requires-Dist: sympy
+Requires-Dist: six
+Requires-Dist: pymatgen
 
 chemcoord: A python module for coordinates of molecules
 =======================================================
 
 
 .. list-table::
    :widths: 25 25
    :header-rows: 0
 
+   * - .. image:: https://github.com/mcocdawc/chemcoord/blob/v2.1.1/docs/source/_static/logo/chemcoord_logo.png
+              :align: center
+              :width: 140
+              :alt: Chemcoord logo
+     -
    * - Latest Release
      - .. image:: https://img.shields.io/pypi/v/chemcoord.svg
             :target: https://pypi.python.org/pypi/chemcoord
    * - Package Status
      - .. image:: https://img.shields.io/pypi/status/chemcoord.svg
             :target: https://pypi.python.org/pypi/chemcoord
    * - Documentation
@@ -82,39 +97,47 @@
    all functions are tested and tailored around the work flow in
    theoretical chemistry.
 -  `It as a python module ;) <https://xkcd.com/353/>`__
 
 Installation guide
 ------------------
 
-A working python 3 installation is required (>=3.7 are possible).
+A working python 3 installation is required (3.7 <= version <= 3.11 are tested).
 
 It is highly recommended to use this module in combination with
 `Ipython <http://ipython.org/>`__ and `jupyter <http://jupyter.org/>`__.
-They come shipped by default with the `anaconda3
-installer <https://www.continuum.io/downloads/>`__
+
 
 Unix
 ~~~~
 
-For the packaged version, the following commands have to be executed in
-the terminal:
+There are packaged versions on PyPi and conda-forge.
+
+For the packaged version from `PyPi <https://pypi.org/project/chemcoord/>`__, the following commands have to be executed:
 
 ::
 
    pip install chemcoord
 
+
+For the packaged version from `conda-forge <https://anaconda.org/conda-forge/chemcoord>`__, the following commands have to be executed:
+
+::
+
+   conda install -c conda-forge chemcoord
+
 For the up to date development version (experimental):
 
 ::
 
    git clone https://github.com/mcocdawc/chemcoord.git
    cd chemcoord
    pip install .
 
+
 Windows
 ~~~~~~~
 
 Neither installation nor running the module are tested on windows. To
 the best of my knowledge it should work there as well. Just use the same
 steps as for UNIX.
 
@@ -139,24 +162,22 @@
         doi = {10.1002/jcc.27029},
         year = {2023}
     }
 
 
 My (Oskar Weser) master thesis including a more detailed derivation of implemented equations and
 the mathematical background can be found
-`here <https://github.com/mcocdawc/chemcoord/blob/master/docs/source/files/master_thesis_oskar_weser_chemcoord.pdf>`__.
+`here <https://github.com/mcocdawc/chemcoord/blob/master/docs/source/_static/master_thesis_oskar_weser_chemcoord.pdf>`__.
 
 
 
 Acknowledgement
 ~~~~~~~~~~~~~~~
 
 
 .. image:: https://github.com/zulip/zulip/blob/main/static/images/logo/zulip-icon-circle.svg
    :width: 80
    :align: left
    :target: https://zulip.com/
 
 Zulip is an open-source modern team chat app designed to keep both live and asynchronous conversations organized,
 that supports the development of chemcoord with a free plan.
-
-
```

### Comparing `chemcoord-2.1.0/README.rst` & `chemcoord-2.1.1/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 =======================================================
 
 
 .. list-table::
    :widths: 25 25
    :header-rows: 0
 
+   * - .. image:: https://github.com/mcocdawc/chemcoord/blob/v2.1.1/docs/source/_static/logo/chemcoord_logo.png
+              :align: center
+              :width: 140
+              :alt: Chemcoord logo
+     -
    * - Latest Release
      - .. image:: https://img.shields.io/pypi/v/chemcoord.svg
             :target: https://pypi.python.org/pypi/chemcoord
    * - Package Status
      - .. image:: https://img.shields.io/pypi/status/chemcoord.svg
             :target: https://pypi.python.org/pypi/chemcoord
    * - Documentation
@@ -56,39 +61,47 @@
    all functions are tested and tailored around the work flow in
    theoretical chemistry.
 -  `It as a python module ;) <https://xkcd.com/353/>`__
 
 Installation guide
 ------------------
 
-A working python 3 installation is required (>=3.7 are possible).
+A working python 3 installation is required (3.7 <= version <= 3.11 are tested).
 
 It is highly recommended to use this module in combination with
 `Ipython <http://ipython.org/>`__ and `jupyter <http://jupyter.org/>`__.
-They come shipped by default with the `anaconda3
-installer <https://www.continuum.io/downloads/>`__
+
 
 Unix
 ~~~~
 
-For the packaged version, the following commands have to be executed in
-the terminal:
+There are packaged versions on PyPi and conda-forge.
+
+For the packaged version from `PyPi <https://pypi.org/project/chemcoord/>`__, the following commands have to be executed:
 
 ::
 
    pip install chemcoord
 
+
+For the packaged version from `conda-forge <https://anaconda.org/conda-forge/chemcoord>`__, the following commands have to be executed:
+
+::
+
+   conda install -c conda-forge chemcoord
+
 For the up to date development version (experimental):
 
 ::
 
    git clone https://github.com/mcocdawc/chemcoord.git
    cd chemcoord
    pip install .
 
+
 Windows
 ~~~~~~~
 
 Neither installation nor running the module are tested on windows. To
 the best of my knowledge it should work there as well. Just use the same
 steps as for UNIX.
 
@@ -113,15 +126,15 @@
         doi = {10.1002/jcc.27029},
         year = {2023}
     }
 
 
 My (Oskar Weser) master thesis including a more detailed derivation of implemented equations and
 the mathematical background can be found
-`here <https://github.com/mcocdawc/chemcoord/blob/master/docs/source/files/master_thesis_oskar_weser_chemcoord.pdf>`__.
+`here <https://github.com/mcocdawc/chemcoord/blob/master/docs/source/_static/master_thesis_oskar_weser_chemcoord.pdf>`__.
 
 
 
 Acknowledgement
 ~~~~~~~~~~~~~~~
```

### Comparing `chemcoord-2.1.0/docs/source/cartesian_coordinates.rst` & `chemcoord-2.1.1/docs/source/cartesian_coordinates.rst`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.0/docs/source/configuration.rst` & `chemcoord-2.1.1/docs/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.0/docs/source/index.rst` & `chemcoord-2.1.1/docs/source/index.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 Welcome to ChemCoord's documentation!
 =====================================
 
+The code can be found `here <https://github.com/mcocdawc/chemcoord>`_.
+
 
 Features
 ++++++++
 
 * Molecules are reliably transformed between cartesian space and
   non redundant internal coordinates (Zmatrices).
   Dummy atoms are inserted and removed automatically on the fly if necessary.
@@ -36,31 +38,52 @@
 .. toctree::
     :maxdepth: 2
 
     installation.rst
     tutorial.rst
     documentation.rst
     references.rst
-    bugs.rst
+    bugs_and_contributors.rst
     license.rst
 
 
 The changelog can be found
 `here <https://github.com/mcocdawc/chemcoord/blob/master/CHANGELOG.md>`_.
 
 Citation and mathematical background
 ++++++++++++++++++++++++++++++++++++
 
-If chemcoord is used in a project that leads to a scientific publication,
-please acknowledge this fact by citing Oskar Weser (2017) using this ready-made BibTeX entry::
+
+The theory behind chemcoord is described in `this paper <https://onlinelibrary.wiley.com/doi/full/10.1002/jcc.27029>`__.
+If this package is used in a project that leads to a scientific
+publication, please acknowledge it by citing.
+
+::
+
+    @article{https://doi.org/10.1002/jcc.27029,
+        author = {Weser, Oskar and Hein-Janke, Björn and Mata, Ricardo A.},
+        title = {Automated handling of complex chemical structures in Z-matrix coordinates—The chemcoord library},
+        journal = {Journal of Computational Chemistry},
+        volume = {44},
+        number = {5},
+        pages = {710-726},
+        keywords = {analytical gradients, geometry optimization, non-linear constraints, transition state search, Z-matrix},
+        doi = {10.1002/jcc.27029},
+        year = {2023}
+    }
+
+
+My (Oskar Weser) master thesis including a more detailed derivation of implemented equations and
+the mathematical background can be found
+`here <https://github.com/mcocdawc/chemcoord/blob/master/docs/source/_static/master_thesis_oskar_weser_chemcoord.pdf>`__.
+It also has a ready-made BibTeX entry:
+
+::
 
   @mastersthesis{OWeser2017,
-  author = {Oskar Weser},
-  title = {An efficient and general library for the definition and use of internal coordinates in large molecular systems},
-  school = {Georg August Universität Göttingen},
-  year = {2017},
-  month = {November},
+      author = {Oskar Weser},
+      title = {An efficient and general library for the definition and use of internal coordinates in large molecular systems},
+      school = {Georg August Universität Göttingen},
+      year = {2017},
+      month = {November},
   }
 
-The master thesis including the derivation of implemented equations
-and the mathematical background can be found
-`here <https://github.com/mcocdawc/chemcoord/blob/master/docs/source/files/master_thesis_oskar_weser_chemcoord.pdf>`_.
```

### Comparing `chemcoord-2.1.0/docs/source/installation.rst` & `chemcoord-2.1.1/docs/source/installation.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Installation guide
 ==================
-A working python 3 installation is required (versions >=3.7 are possible).
+A working python 3 installation is required (3.7 <= version <= 3.11 are tested).
 
 It is highly recommended to use this module in combination with
 `Ipython <http://ipython.org/>`_ and `jupyter <http://jupyter.org/>`_.
 They come shipped by default with the
 `anaconda3 installer <https://www.continuum.io/downloads/>`_.
 
 Unix
 ++++
 
 
-For the packaged versions, the following commands have to be executed in the
-terminal::
+There are packaged versions on PyPi and conda-forge.
 
-  conda install -c mcocdawc chemcoord
+For the packaged version from `PyPi <https://pypi.org/project/chemcoord/>`__, the following commands have to be executed::
 
-or::
+   pip install chemcoord
 
-  pip install chemcoord
 
+For the packaged version from `conda-forge <https://anaconda.org/conda-forge/chemcoord>`__, the following commands have to be executed::
+
+   conda install -c conda-forge chemcoord
 
 For the up to date development version (experimental)::
 
-  git clone https://github.com/mcocdawc/chemcoord.git
-  cd chemcoord
-  pip install .
+   git clone https://github.com/mcocdawc/chemcoord.git
+   cd chemcoord
+   pip install .
 
 Windows
 +++++++
 
 Neither installation nor running the module are tested on windows.
 To the best of my knowledge it should work there as well.
 Just use the same steps as for UNIX.
```

### Comparing `chemcoord-2.1.0/docs/source/internal_coordinates.rst` & `chemcoord-2.1.1/docs/source/internal_coordinates.rst`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.0/docs/source/license.rst` & `chemcoord-2.1.1/docs/source/license.rst`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.0/docs/source/references.rst` & `chemcoord-2.1.1/docs/source/references.rst`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.0/docs/source/tutorial.rst` & `chemcoord-2.1.1/docs/source/tutorial.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Tutorial
 ==================
 
 Just follow the link to the example notebooks.
 
 
-  * `Cartesian <http://nbviewer.jupyter.org/github/mcocdawc/chemcoord/blob/v2.1.0/Tutorial/Cartesian.ipynb>`_
-  * `Zmat <http://nbviewer.jupyter.org/github/mcocdawc/chemcoord/blob/v2.1.0/Tutorial/Zmat.ipynb>`_
-  * `Transformation <http://nbviewer.jupyter.org/github/mcocdawc/chemcoord/blob/v2.1.0/Tutorial/Transformation.ipynb>`_
-  * `Gradients <http://nbviewer.jupyter.org/github/mcocdawc/chemcoord/blob/v2.1.0/Tutorial/Gradients.ipynb>`_
-  * `Advanced customisation <http://nbviewer.jupyter.org/github/mcocdawc/chemcoord/blob/v2.1.0/Tutorial/Advanced_customisation.ipynb>`_
+  * `Cartesian <http://nbviewer.jupyter.org/github/mcocdawc/chemcoord/blob/v2.1.1/Tutorial/Cartesian.ipynb>`_
+  * `Zmat <http://nbviewer.jupyter.org/github/mcocdawc/chemcoord/blob/v2.1.1/Tutorial/Zmat.ipynb>`_
+  * `Transformation <http://nbviewer.jupyter.org/github/mcocdawc/chemcoord/blob/v2.1.1/Tutorial/Transformation.ipynb>`_
+  * `Gradients <http://nbviewer.jupyter.org/github/mcocdawc/chemcoord/blob/v2.1.1/Tutorial/Gradients.ipynb>`_
+  * `Advanced customisation <http://nbviewer.jupyter.org/github/mcocdawc/chemcoord/blob/v2.1.1/Tutorial/Advanced_customisation.ipynb>`_
 
 If you want to have an interactive session, just download the following
-`zip file <https://minhaskamal.github.io/DownGit/#/home?url=https://github.com/mcocdawc/chemcoord/tree/v2.1.0/Tutorial>`_,
+`zip file <https://minhaskamal.github.io/DownGit/#/home?url=https://github.com/mcocdawc/chemcoord/tree/v2.1.1/Tutorial>`_,
 which contains all notebooks and coordinates.
```

### Comparing `chemcoord-2.1.0/setup.py` & `chemcoord-2.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,17 +27,19 @@
     'Operating System :: POSIX',
     'Operating System :: Microsoft :: Windows',
     'Natural Language :: English',
     'Programming Language :: Python',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
     'Topic :: Scientific/Engineering :: Chemistry',
     'Topic :: Scientific/Engineering :: Physics']
-VERSION = '2.1.0'
+VERSION = '2.1.1'
 
 
 def readme():
     '''Return the contents of the README.md file.'''
     with open('README.rst') as freadme:
         return freadme.read()
 
@@ -49,14 +51,15 @@
         url=URL,
         description=DESCRIPTION,
         author=AUTHOR,
         author_email=EMAIL,
         include_package_data=True,
         keywords=KEYWORDS,
         license=LICENSE,
+        long_description_content_type="text/x-rst",
         long_description=readme(),
         classifiers=CLASSIFIERS,
         packages=find_packages('src'),
         package_dir={'': 'src'},
         install_requires=INSTALL_REQUIRES,
     )
```

### Comparing `chemcoord-2.1.0/src/chemcoord/__init__.py` & `chemcoord-2.1.1/src/chemcoord/__init__.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.0/src/chemcoord/_generic_classes/generic_core.py` & `chemcoord-2.1.1/src/chemcoord/_generic_classes/generic_core.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/_cart_transformation.py` & `chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/_cart_transformation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,48 +1,57 @@
 # -*- coding: utf-8 -*-
 import warnings
 
 import numba as nb
+from numba import jit
 from numba.core.errors import NumbaDeprecationWarning
-from numba import jit, generated_jit
+from numba.extending import overload
 import numpy as np
 from numpy import arccos, arctan2, sqrt
 
 import chemcoord.constants as constants
 from chemcoord.cartesian_coordinates.xyz_functions import (_jit_cross,
                                                            _jit_isclose,
                                                            _jit_normalize)
 from chemcoord.exceptions import ERR_CODE_OK, ERR_CODE_InvalidReference
 
 
-with warnings.catch_warnings():
-    # This has to be fixed in the near-future
-    # https://github.com/mcocdawc/chemcoord/issues/76
-    warnings.simplefilter("ignore", category=NumbaDeprecationWarning)
-    @generated_jit(nopython=True)
-    def get_ref_pos(X, indices):  # pylint:disable=unused-argument
-        if isinstance(indices, nb.types.Array):
-            def f(X, indices):
-                ref_pos = np.empty((3, len(indices)))
-                for col, i in enumerate(indices):
-                    if i < constants.keys_below_are_abs_refs:
-                        ref_pos[:, col] = constants._jit_absolute_refs(i)
-                    else:
-                        ref_pos[:, col] = X[:, i]
-                return ref_pos
-            return f
-        elif isinstance(indices, nb.types.Integer):
-            def f(X, indices):
-                i = indices
+
+def _stub_get_ref_pos(X, indices):  # pylint:disable=unused-argument
+    raise AssertionError("Should not call this function unjitted.")
+
+
+@overload(_stub_get_ref_pos)
+def _get_ref_pos_impl(X, indices):  # pylint:disable=unused-argument
+    if isinstance(indices, nb.types.Array):
+        def f(X, indices):
+            ref_pos = np.empty((3, len(indices)))
+            for col, i in enumerate(indices):
                 if i < constants.keys_below_are_abs_refs:
-                    ref_pos = constants._jit_absolute_refs(i)
+                    ref_pos[:, col] = constants._jit_absolute_refs(i)
                 else:
-                    ref_pos = X[:, i]
-                return ref_pos
-            return f
+                    ref_pos[:, col] = X[:, i]
+            return ref_pos
+        return f
+    elif isinstance(indices, nb.types.Integer):
+        def f(X, indices):
+            i = indices
+            if i < constants.keys_below_are_abs_refs:
+                ref_pos = constants._jit_absolute_refs(i)
+            else:
+                ref_pos = X[:, i]
+            return ref_pos
+        return f
+    else:
+        raise AssertionError("Should not be here")
+
+
+@jit(nopython=True, cache=True)
+def get_ref_pos(X, indices):
+    return _stub_get_ref_pos(X, indices)
 
 
 @jit(nopython=True, cache=True)
 def get_B(X, c_table, j):
     B = np.empty((3, 3))
     ref_pos = get_ref_pos(X, c_table[:, j])
     BA = ref_pos[:, 1] - ref_pos[:, 0]
```

### Comparing `chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/_cartesian_class_core.py` & `chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/_cartesian_class_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,16 +52,16 @@
                 == bool(atoms is not None and coords is not None)):
             message = 'atoms and coords have to be both None or not None'
             raise IllegalArgumentCombination(message)
         elif frame is None and atoms is None and coords is None:
             message = 'Either frame or atoms and coords have to be not None'
             raise IllegalArgumentCombination(message)
         elif atoms is not None and coords is not None:
-            frame = pd.DataFrame(index=index,
-                                 columns=['atom', 'x', 'y', 'z'], dtype='f8')
+            dtypes = [('atom', str), ('x', float), ('y', float), ('z', float)]
+            frame = pd.DataFrame(np.empty(len(atoms), dtype=dtypes), index=index)
             frame['atom'] = atoms
             frame.loc[:, ['x', 'y', 'z']] = coords
         elif not isinstance(frame, pd.DataFrame):
             raise ValueError('Need a pd.DataFrame as input')
         if not self._required_cols <= set(frame.columns):
             raise PhysicalMeaning('There are columns missing for a '
                                   'meaningful description of a molecule')
@@ -91,15 +91,15 @@
             molecule._metadata = copy.deepcopy(self._metadata)
             return molecule
         else:
             return selected
 
     def _test_if_can_be_added(self, other):
         if not (set(self.index) == set(other.index)
-                and np.alltrue(self['atom'] == other.loc[self.index, 'atom'])):
+                and (self['atom'] == other.loc[self.index, 'atom']).all(axis=None)):
             message = ("You can add only Cartesians which are indexed in the "
                        "same way and use the same atoms.")
             raise PhysicalMeaning(message)
 
     def __add__(self, other):
         coords = ['x', 'y', 'z']
         new = self.copy()
@@ -231,18 +231,14 @@
 
     def __eq__(self, other):
         return self._frame == other._frame
 
     def __ne__(self, other):
         return self._frame != other._frame
 
-    def _to_numeric(self):
-        return self.__class__(self._frame.apply(
-            partial(pd.to_numeric, errors='ignore')))
-
     def copy(self):
         molecule = self.__class__(self._frame)
         molecule.metadata = self.metadata.copy()
         molecule._metadata = copy.deepcopy(self._metadata)
         return molecule
 
     def subs(self, *args):
@@ -281,15 +277,15 @@
                 return x
             return subs_function
 
         for col in cols:
             if out.loc[:, col].dtype is np.dtype('O'):
                 out.loc[:, col] = out.loc[:, col].map(get_subs_f(*args))
                 try:
-                    out.loc[:, col] = out.loc[:, col].astype('f8')
+                    out._frame = out._frame.astype({col: 'f8'})
                 except (SystemError, TypeError):
                     pass
         return out
 
     @staticmethod
     @jit(nopython=True, cache=True)
     def _jit_give_bond_array(pos, bond_radii, self_bonding_allowed=False):
```

### Comparing `chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/_cartesian_class_get_zmat.py` & `chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/_cartesian_class_get_zmat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 import warnings
 from collections import OrderedDict
+
 from functools import partial
 from itertools import permutations
 
 import numpy as np
 import pandas as pd
 from numba.core.errors import NumbaPerformanceWarning
 
@@ -13,14 +14,15 @@
 import chemcoord.constants as constants
 from chemcoord.cartesian_coordinates._cartesian_class_core import CartesianCore
 from chemcoord.configuration import settings
 from chemcoord.exceptions import (ERR_CODE_OK, ERR_CODE_InvalidReference,
                                   IllegalArgumentCombination, InvalidReference,
                                   UndefinedCoordinateSystem)
 from chemcoord.internal_coordinates.zmat_class_main import Zmat
+from chemcoord.utilities._temporary_deprecation_workarounds import replace_without_warn
 
 
 class CartesianGetZmat(CartesianCore):
     @staticmethod
     def _check_construction_table(construction_table):
         """Checks if a construction table uses valid references.
         Raises an exception (UndefinedCoordinateSystem) otherwise.
@@ -484,15 +486,16 @@
             else:
                 c_table = np.array(c_table)
                 if len(c_table.shape) == 1:
                     c_table = c_table[None, :]
                 c_table = pd.DataFrame(
                     data=c_table[:, 1:], index=c_table[:, 0],
                     columns=['b', 'a', 'd'])
-        c_table = c_table.replace(constants.int_label).astype('i8')
+
+        c_table = replace_without_warn(c_table, constants.int_label).astype('i8')
         c_table.index = c_table.index.astype('i8')
 
         new_index = c_table.index.append(self.index.difference(c_table.index))
         X = self.loc[new_index, ['x', 'y', 'z']].values.astype('f8').T
         c_table = c_table.replace(dict(zip(new_index, range(len(self)))))
         c_table = c_table.values.T
 
@@ -507,29 +510,31 @@
         Args:
             Construction table (pd.DataFrame):
 
         Returns:
             Zmat: A new instance of :class:`Zmat`.
         """
         c_table = construction_table
-        default_cols = ['atom', 'b', 'bond', 'a', 'angle', 'd', 'dihedral']
-        optional_cols = list(set(self.columns) - {'atom', 'x', 'y', 'z'})
+        dtypes = [('atom', str),
+                        ('b', str), ('bond', float),
+                        ('a', str), ('angle', float),
+                        ('d', str), ('dihedral', float)]
 
-        zmat_frame = pd.DataFrame(columns=default_cols + optional_cols,
-                                  dtype='float', index=c_table.index)
-
-        zmat_frame.loc[:, optional_cols] = self.loc[c_table.index,
-                                                    optional_cols]
+        zmat_frame = pd.DataFrame(np.empty(len(c_table), dtype=dtypes),
+                                  index=c_table.index)
 
         zmat_frame.loc[:, 'atom'] = self.loc[c_table.index, 'atom']
         zmat_frame.loc[:, ['b', 'a', 'd']] = c_table
 
         zmat_values = self._calculate_zmat_values(c_table)
         zmat_frame.loc[:, ['bond', 'angle', 'dihedral']] = zmat_values
 
+        zmat_frame = zmat_frame.join(
+            self._frame.loc[:, list(set(self.columns) - {'atom', 'x', 'y', 'z'})])
+
         zmatrix = Zmat(zmat_frame, metadata=self.metadata,
                        _metadata={'last_valid_cartesian': self.copy()})
         return zmatrix
 
     def get_zmat(self, construction_table=None,
                  use_lookup=None):
         """Transform to internal coordinates.
@@ -687,17 +692,21 @@
             :func:`~chemcoord.xyz_functions.apply_grad_zmat_tensor`
             with partially replaced arguments.
         """
         if (construction_table.index != self.index).any():
             message = "construction_table and self must use the same index"
             raise ValueError(message)
         c_table = construction_table.loc[:, ['b', 'a', 'd']]
-        c_table = c_table.replace(constants.int_label)
-        c_table = c_table.replace({k: v for v, k in enumerate(c_table.index)})
-        c_table = c_table.values.T
+
+
+        c_table = (replace_without_warn(c_table, constants.int_label)
+                        .astype('i8')
+                        .replace({k: v for v, k in enumerate(c_table.index)})
+                        .values
+                        .T)
         X = self.loc[:, ['x', 'y', 'z']].values.T
         if X.dtype == np.dtype('i8'):
             X = X.astype('f8')
 
         with warnings.catch_warnings():
             # There were some performance warnings about non-contiguos arrays.
             # Unfortunately we cannot do anything about it, on a conceptional level.
```

### Comparing `chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/_cartesian_class_io.py` & `chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/_cartesian_class_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -355,17 +355,16 @@
 
         Args:
             molecule (:class:`pymatgen.core.structure.Molecule`):
 
         Returns:
             Cartesian:
         """
-        new = cls(atoms=[el.value for el in molecule.species],
-                  coords=molecule.cart_coords)
-        return new._to_numeric()
+        return cls(atoms=[el.value for el in molecule.species],
+                   coords=molecule.cart_coords)
 
     def get_ase_atoms(self):
         """Create an Atoms instance of the ase library
 
         .. warning:: The `ase library <https://wiki.fysik.dtu.dk/ase/>`_
             is imported locally in this function and will raise
             an ``ImportError`` exception, if it is not installed.
```

### Comparing `chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/_cartesian_class_pandas_wrapper.py` & `chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/_cartesian_class_pandas_wrapper.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/_cartesian_class_symmetry.py` & `chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/_cartesian_class_symmetry.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         eq['eq_sets'] = {rename[k]: {rename[x] for x in v}
                          for k, v in eq['eq_sets'].items()}
         eq['sym_ops'] = {rename[k]: {rename[x]: v[x] for x in v}
                          for k, v in eq['sym_ops'].items()}
         try:
             sym_mol = self.from_pymatgen_molecule(eq['sym_mol'])
             sym_mol.index = self.index
-            eq['sym_mol'] = sym_mol._to_numeric()
+            eq['sym_mol'] = sym_mol
         except KeyError:
             pass
 
     def get_pointgroup(self, tolerance=0.3):
         """Returns a PointGroup object for the molecule.
 
         Args:
```

### Comparing `chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/asymmetric_unit_cartesian_class.py` & `chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/asymmetric_unit_cartesian_class.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/cartesian_class_main.py` & `chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/cartesian_class_main.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/point_group.py` & `chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/point_group.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/xyz_functions.py` & `chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/xyz_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -196,24 +196,25 @@
             look into :func:`numpy.isclose` for further explanation.
 
     Returns:
         :class:`numpy.ndarray`: Boolean array.
     """
     coords = ['x', 'y', 'z']
     if not (set(a.index) == set(b.index)
-            and np.alltrue(a.loc[:, 'atom'] == b.loc[a.index, 'atom'])):
+            and (a.loc[:, 'atom'] == b.loc[a.index, 'atom']).all(axis=None)):
         message = 'Can only compare molecules with the same atoms and labels'
         raise ValueError(message)
 
     if align:
         a = a.get_inertia()['transformed_Cartesian']
         b = b.get_inertia()['transformed_Cartesian']
     A, B = a.loc[:, coords], b.loc[a.index, coords]
-    out = a._frame.copy()
-    out['atom'] = True
+
+    out = pd.DataFrame(index=a.index, columns=['atom'] + coords, dtype=bool)
+    out.loc[:, 'atom'] = True
     out.loc[:, coords] = np.isclose(A, B, rtol=rtol, atol=atol)
     return out
 
 
 def allclose(a, b, align=False, rtol=1.e-5, atol=1.e-8):
     """Compare two molecules for numerical equality.
 
@@ -227,15 +228,15 @@
             look into :func:`numpy.allclose` for further explanation.
         atol (float): Relative tolerance for the numerical equality comparison
             look into :func:`numpy.allclose` for further explanation.
 
     Returns:
         bool:
     """
-    return np.alltrue(isclose(a, b, align=align, rtol=rtol, atol=atol))
+    return isclose(a, b, align=align, rtol=rtol, atol=atol).all(axis=None)
 
 
 def concat(cartesians, ignore_index=False, keys=None):
     """Join list of cartesians into one molecule.
 
     Wrapper around the :func:`pandas.concat` function.
     Default values are the same as in the pandas function except for
@@ -461,29 +462,33 @@
 
     Returns:
         :class:`Zmat`: Distortions in Zmatrix space.
     """
     if (construction_table.index != cart_dist.index).any():
         message = "construction_table and cart_dist must use the same index"
         raise ValueError(message)
+    from chemcoord.internal_coordinates.zmat_class_main import Zmat
+    dtypes = [('atom', str),
+                    ('b', str), ('bond', float),
+                    ('a', str), ('angle', float),
+                    ('d', str), ('dihedral', float)]
+
+    new = pd.DataFrame(np.empty(len(construction_table), dtype=dtypes),
+                              index=cart_dist.index)
+
     X_dist = cart_dist.loc[:, ['x', 'y', 'z']].values.T
     C_dist = np.tensordot(grad_C, X_dist, axes=([3, 2], [0, 1])).T
     if C_dist.dtype == np.dtype('i8'):
         C_dist = C_dist.astype('f8')
     try:
         C_dist[:, [1, 2]] = np.rad2deg(C_dist[:, [1, 2]])
     # Unevaluated symbolic expressions are remaining.
     # catches AttributeError as well, because this was
     # the raised exception before https://github.com/numpy/numpy/issues/13666
     except (AttributeError, TypeError):
         C_dist[:, [1, 2]] = sympy.deg(C_dist[:, [1, 2]])
+        new = new.astype({k: 'O' for k in ['bond', 'angle', 'dihedral']})
 
-    from chemcoord.internal_coordinates.zmat_class_main import Zmat
-    cols = ['atom', 'b', 'bond', 'a', 'angle', 'd', 'dihedral']
-    dtypes = ['O', 'i8', 'f8', 'i8', 'f8', 'i8', 'f8']
-    new = pd.DataFrame(data=np.zeros((len(construction_table), 7)),
-                       index=cart_dist.index, columns=cols, dtype='f8')
-    new = new.astype(dict(zip(cols, dtypes)))
     new.loc[:, ['b', 'a', 'd']] = construction_table
     new.loc[:, 'atom'] = cart_dist.loc[:, 'atom']
     new.loc[:, ['bond', 'angle', 'dihedral']] = C_dist
     return Zmat(new, _metadata={'last_valid_cartesian': cart_dist})
```

### Comparing `chemcoord-2.1.0/src/chemcoord/configuration.py` & `chemcoord-2.1.1/src/chemcoord/configuration.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.0/src/chemcoord/constants.py` & `chemcoord-2.1.1/src/chemcoord/constants.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.0/src/chemcoord/exceptions.py` & `chemcoord-2.1.1/src/chemcoord/exceptions.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.0/src/chemcoord/internal_coordinates/_zmat_class_core.py` & `chemcoord-2.1.1/src/chemcoord/internal_coordinates/_zmat_class_core.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import pandas as pd
 from chemcoord._generic_classes.generic_core import GenericCore
 from chemcoord.exceptions import (ERR_CODE_OK, ERR_CODE_InvalidReference,
                                   InvalidReference, PhysicalMeaning)
 from chemcoord.internal_coordinates._zmat_class_pandas_wrapper import \
     PandasWrapper
 from chemcoord.utilities import _decorators
+from chemcoord.utilities._temporary_deprecation_workarounds import replace_without_warn
 
 append_indexer_docstring = _decorators.Appender(
     """In the case of obtaining elements, the indexing behaves like
 Indexing and Selecting data in
 `Pandas <http://pandas.pydata.org/pandas-docs/stable/indexing.html>`_.
 
 For assigning elements it is necessary to make a explicit decision
@@ -148,16 +149,16 @@
         """Integer position based indexing for obtaining elements
 and assigning values safely.
         """
         return indexers._Safe_ILoc(self)
 
     def _test_if_can_be_added(self, other):
         cols = ['atom', 'b', 'a', 'd']
-        if not (np.alltrue(self.loc[:, cols] == other.loc[:, cols])
-                and np.alltrue(self.index == other.index)):
+        if not ((self.loc[:, cols] == other.loc[:, cols]).all(axis=None)
+                and (self.index == other.index).all()):
             message = ("You can add only those zmatrices that have the same "
                        "index, use the same construction table, have the same "
                        "ordering... The only allowed difference is in the "
                        "columns ['bond', 'angle', 'dihedral']")
             raise PhysicalMeaning(message)
 
     def __add__(self, other):
@@ -288,35 +289,35 @@
         zmat_values = ['bond', 'angle', 'dihedral']
         new.loc[:, zmat_values] = frame.loc[:, zmat_values].astype('f8')
         zmat_cols = ['b', 'a', 'd']
         new.loc[:, zmat_cols] = frame.loc[:, zmat_cols].astype('i8')
         return new
 
     def iupacify(self):
-        """Give the IUPAC conform representation.
+        r"""Give the IUPAC conform representation.
 
         Mathematically speaking the angles in a zmatrix are
         representations of an equivalence class.
-        We will denote an equivalence relation with :math:`\\sim`
-        and use :math:`\\alpha` for an angle and :math:`\\delta` for a dihedral
+        We will denote an equivalence relation with :math:`\sim`
+        and use :math:`\alpha` for an angle and :math:`\delta` for a dihedral
         angle. Then the following equations hold true.
 
         .. math::
 
-           (\\alpha, \\delta) &\sim (-\\alpha, \\delta + \\pi) \\\\
-           \\alpha &\sim \\alpha \\mod 2\\pi \\\\
-           \\delta &\sim \\delta \\mod 2\\pi
+           (\alpha, \delta) &\sim (-\alpha, \delta + \pi) \\
+           \alpha &\sim \alpha \mod 2\pi \\
+           \delta &\sim \delta \mod 2\pi
 
         `IUPAC <https://goldbook.iupac.org/html/T/T06406.html>`_ defines
         a designated representation of these equivalence classes, by asserting:
 
         .. math::
 
-           0 \\leq &\\alpha \\leq \\pi \\\\
-           -\\pi \\leq &\\delta \\leq \\pi
+           0 \leq &\alpha \leq \pi \\
+           -\pi \leq &\delta \leq \pi
 
         Args:
             None
 
         Returns:
             Zmat: Zmatrix with accordingly changed angles and dihedrals.
         """
@@ -433,15 +434,15 @@
                 return x
             return subs_function
 
         for col in cols:
             if out.loc[:, col].dtype is np.dtype('O'):
                 out.unsafe_loc[:, col] = out.loc[:, col].map(get_subs_f(*args))
                 try:
-                    out._frame[col] = out.loc[:, col].astype('f8')
+                    out._frame = out._frame.astype({col: 'f8'})
                 except (SystemError, TypeError):
                     pass
         if perform_checks:
             try:
                 new_cartesian = out.get_cartesian()
             except (AttributeError, TypeError):
                 # Unevaluated symbolic expressions are remaining.
@@ -485,15 +486,15 @@
         # Transtitive [1].replace(A) gives [3]
         # Non-Transtitive [1].replace(A) gives [2]
         # https://github.com/pandas-dev/pandas/issues/5338
         # https://github.com/pandas-dev/pandas/issues/16051
         # https://github.com/pandas-dev/pandas/issues/5541
         # For this reason convert to int and replace then.
 
-        c_table = c_table.replace(constants.int_label)
+        c_table = replace_without_warn(c_table, constants.int_label)
         try:
             c_table = c_table.astype('i8')
         except ValueError:
             raise ValueError('Due to a bug in pandas it is necessary to have '
                              'integer columns')
         c_table = c_table.replace(self.index, new_index)
         c_table = c_table.replace(
@@ -650,17 +651,19 @@
             xyz_frame.loc[:, ['x', 'y', 'z']] = positions[:row]
             from chemcoord.cartesian_coordinates.cartesian_class_main \
                 import Cartesian
             cartesian = Cartesian(xyz_frame, metadata=self.metadata)
             return cartesian
 
         c_table = self.loc[:, ['b', 'a', 'd']]
-        c_table = c_table.replace(constants.int_label)
-        c_table = c_table.replace({k: v for v, k in enumerate(c_table.index)})
-        c_table = c_table.values.astype('i8').T
+        c_table = (replace_without_warn(c_table, constants.int_label)
+                    .astype('i8')
+                    .replace({k: v for v, k in enumerate(c_table.index)})
+                    .values
+                    .T)
 
         C = self.loc[:, ['bond', 'angle', 'dihedral']].values.T
         C[[1, 2], :] = np.radians(C[[1, 2], :])
 
         err, row, positions = transformation.get_X(C, c_table)
         positions = positions.T
 
@@ -763,16 +766,21 @@
         Returns:
             (func, :class:`numpy.ndarray`): Depending on ``as_function``
             return a tensor or
             :func:`~chemcoord.zmat_functions.apply_grad_cartesian_tensor`
             with partially replaced arguments.
         """
         zmat = self.change_numbering()
-        c_table = zmat.loc[:, ['b', 'a', 'd']]
-        c_table = c_table.replace(constants.int_label).values.T
+
+        c_table = (replace_without_warn(zmat.loc[:, ['b', 'a', 'd']],
+                                        constants.int_label)
+                    .astype('i8')
+                    .values
+                    .T)
+
         C = zmat.loc[:, ['bond', 'angle', 'dihedral']].values.T
         if C.dtype == np.dtype('i8'):
             C = C.astype('f8')
         C[[1, 2], :] = np.radians(C[[1, 2], :])
 
 
         grad_X = transformation.get_grad_X(C, c_table, chain=chain)
```

### Comparing `chemcoord-2.1.0/src/chemcoord/internal_coordinates/_zmat_class_io.py` & `chemcoord-2.1.1/src/chemcoord/internal_coordinates/_zmat_class_io.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,14 +39,15 @@
             return (insert_txt + substr).join(txt.split(substr))
         html_txt = out._frame._repr_html_()
         insert_txt = '<caption>{}</caption>\n'.format(self.__class__.__name__)
         return insert_before_substring(insert_txt, '<thead>', html_txt)
 
     def _remove_upper_triangle(self):
         out = self.copy()
+        out._frame = out._frame.astype({k: str for k in ['b', 'bond', 'a', 'angle', 'd', 'dihedral']})
         for i in range(min(len(self), 3)):
             out.unsafe_iloc[i, (2 * i + 1):] = ''
         return out
 
     def to_string(self, buf=None, format_abs_ref_as='string',
                   upper_triangle=True, header=True, index=True, **kwargs):
         """Render a DataFrame to a console-friendly tabular output.
@@ -109,15 +110,15 @@
             zmat_frame.index.name = None
         if pd.isnull(zmat_frame.iloc[0, 1]):
             zmat_values = [1.27, 127., 127.]
             zmat_refs = [constants.int_label[x] for x in
                          ['origin', 'e_z', 'e_x']]
             for row, i in enumerate(zmat_frame.index[:3]):
                 cols = ['b', 'a', 'd']
-                zmat_frame.loc[:, cols] = zmat_frame.loc[:, cols].astype('O')
+                zmat_frame = zmat_frame.astype({k: 'O' for k in cols})
                 if row < 2:
                     zmat_frame.loc[i, cols[row:]] = zmat_refs[row:]
                     zmat_frame.loc[i, ['bond', 'angle', 'dihedral'][row:]
                                    ] = zmat_values[row:]
                 else:
                     zmat_frame.loc[i, 'd'] = zmat_refs[2]
                     zmat_frame.loc[i, 'dihedral'] = zmat_values[2]
```

### Comparing `chemcoord-2.1.0/src/chemcoord/internal_coordinates/_zmat_class_pandas_wrapper.py` & `chemcoord-2.1.1/src/chemcoord/internal_coordinates/_zmat_class_pandas_wrapper.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.0/src/chemcoord/internal_coordinates/_zmat_transformation.py` & `chemcoord-2.1.1/src/chemcoord/internal_coordinates/_zmat_transformation.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.0/src/chemcoord/internal_coordinates/zmat_class_main.py` & `chemcoord-2.1.1/src/chemcoord/internal_coordinates/zmat_class_main.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.0/src/chemcoord/internal_coordinates/zmat_functions.py` & `chemcoord-2.1.1/src/chemcoord/internal_coordinates/zmat_functions.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.0/src/chemcoord/utilities/_decorators.py` & `chemcoord-2.1.1/src/chemcoord/utilities/_decorators.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.0/src/chemcoord/utilities/_print_versions.py` & `chemcoord-2.1.1/src/chemcoord/utilities/_print_versions.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.0/src/chemcoord.egg-info/PKG-INFO` & `chemcoord-2.1.1/src/chemcoord.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,56 @@
 Metadata-Version: 2.1
 Name: chemcoord
-Version: 2.1.0
+Version: 2.1.1
 Summary: Python module for dealing with chemical coordinates.
 Home-page: https://github.com/mcocdawc/chemcoord
 Author: Oskar Weser
 Author-email: oskar.weser@gmail.com
 License: LGPLv3
 Keywords: chemcoord,transformation,cartesian,internal,chemistry,zmatrix,xyz,zmat,coordinates,coordinate system
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
+Description-Content-Type: text/x-rst
 License-File: LICENSE.md
+Requires-Dist: numpy>=1.0
+Requires-Dist: scipy
+Requires-Dist: pandas>=1.0
+Requires-Dist: numba>=0.35
+Requires-Dist: sortedcontainers
+Requires-Dist: sympy
+Requires-Dist: six
+Requires-Dist: pymatgen
 
 chemcoord: A python module for coordinates of molecules
 =======================================================
 
 
 .. list-table::
    :widths: 25 25
    :header-rows: 0
 
+   * - .. image:: https://github.com/mcocdawc/chemcoord/blob/v2.1.1/docs/source/_static/logo/chemcoord_logo.png
+              :align: center
+              :width: 140
+              :alt: Chemcoord logo
+     -
    * - Latest Release
      - .. image:: https://img.shields.io/pypi/v/chemcoord.svg
             :target: https://pypi.python.org/pypi/chemcoord
    * - Package Status
      - .. image:: https://img.shields.io/pypi/status/chemcoord.svg
             :target: https://pypi.python.org/pypi/chemcoord
    * - Documentation
@@ -82,39 +97,47 @@
    all functions are tested and tailored around the work flow in
    theoretical chemistry.
 -  `It as a python module ;) <https://xkcd.com/353/>`__
 
 Installation guide
 ------------------
 
-A working python 3 installation is required (>=3.7 are possible).
+A working python 3 installation is required (3.7 <= version <= 3.11 are tested).
 
 It is highly recommended to use this module in combination with
 `Ipython <http://ipython.org/>`__ and `jupyter <http://jupyter.org/>`__.
-They come shipped by default with the `anaconda3
-installer <https://www.continuum.io/downloads/>`__
+
 
 Unix
 ~~~~
 
-For the packaged version, the following commands have to be executed in
-the terminal:
+There are packaged versions on PyPi and conda-forge.
+
+For the packaged version from `PyPi <https://pypi.org/project/chemcoord/>`__, the following commands have to be executed:
 
 ::
 
    pip install chemcoord
 
+
+For the packaged version from `conda-forge <https://anaconda.org/conda-forge/chemcoord>`__, the following commands have to be executed:
+
+::
+
+   conda install -c conda-forge chemcoord
+
 For the up to date development version (experimental):
 
 ::
 
    git clone https://github.com/mcocdawc/chemcoord.git
    cd chemcoord
    pip install .
 
+
 Windows
 ~~~~~~~
 
 Neither installation nor running the module are tested on windows. To
 the best of my knowledge it should work there as well. Just use the same
 steps as for UNIX.
 
@@ -139,24 +162,22 @@
         doi = {10.1002/jcc.27029},
         year = {2023}
     }
 
 
 My (Oskar Weser) master thesis including a more detailed derivation of implemented equations and
 the mathematical background can be found
-`here <https://github.com/mcocdawc/chemcoord/blob/master/docs/source/files/master_thesis_oskar_weser_chemcoord.pdf>`__.
+`here <https://github.com/mcocdawc/chemcoord/blob/master/docs/source/_static/master_thesis_oskar_weser_chemcoord.pdf>`__.
 
 
 
 Acknowledgement
 ~~~~~~~~~~~~~~~
 
 
 .. image:: https://github.com/zulip/zulip/blob/main/static/images/logo/zulip-icon-circle.svg
    :width: 80
    :align: left
    :target: https://zulip.com/
 
 Zulip is an open-source modern team chat app designed to keep both live and asynchronous conversations organized,
 that supports the development of chemcoord with a free plan.
-
-
```

### Comparing `chemcoord-2.1.0/src/chemcoord.egg-info/SOURCES.txt` & `chemcoord-2.1.1/src/chemcoord.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 CHANGELOG.md
 LICENSE.md
 MANIFEST.in
 README.rst
 setup.py
-docs/source/bugs.rst
+docs/source/bugs_and_contributors.rst
 docs/source/cartesian_coordinates.rst
 docs/source/configuration.rst
 docs/source/documentation.rst
 docs/source/exceptions.rst
 docs/source/index.rst
 docs/source/installation.rst
 docs/source/internal_coordinates.rst
@@ -18,15 +18,14 @@
 docs/source/src_AsymmetricUnitCartesian/src_AsymmetricUnitCartesian/chemcoord.AsymmetricUnitCartesian.get_cartesian.rst
 docs/source/src_Cartesian/chemcoord.Cartesian.rst
 docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.__init__.rst
 docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian._divide_et_impera.rst
 docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian._preserve_bonds.rst
 docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.add_data.rst
 docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.align.rst
-docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.append.rst
 docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.basistransform.rst
 docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.change_numbering.rst
 docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.check_absolute_refs.rst
 docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.check_dihedral.rst
 docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.columns.rst
 docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.copy.rst
 docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.correct_absolute_refs.rst
@@ -162,8 +161,9 @@
 src/chemcoord/internal_coordinates/_zmat_class_io.py
 src/chemcoord/internal_coordinates/_zmat_class_pandas_wrapper.py
 src/chemcoord/internal_coordinates/_zmat_transformation.py
 src/chemcoord/internal_coordinates/zmat_class_main.py
 src/chemcoord/internal_coordinates/zmat_functions.py
 src/chemcoord/utilities/__init__.py
 src/chemcoord/utilities/_decorators.py
-src/chemcoord/utilities/_print_versions.py
+src/chemcoord/utilities/_print_versions.py
+src/chemcoord/utilities/_temporary_deprecation_workarounds.py
```

